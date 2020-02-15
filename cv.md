### Hi there! It's my first Junior Developer Resume, well, let's start!

#### 1. Nadezhda Shatalova
#### 2. There is some ways to contact me:
* [Link to VK profile](https://vk.com/little_strange_owl)
* [Link to Github account](https://github.com/owlet1997)
* +79276131173
#### 3. Summary 
As for me it's the most difficult part of task. My goal now is to find my own way in IT-sphere,
because there are a lot of opportunites and jobs here. If we are talking about wishes,
I really don't wanna work with customers like a business analytic.
#### 4. Skills 
* Java
  * Hibernate and JPA
* C++
* Git
#### 5. Code examples 
Okay, let it be the function doPost() from one of servlets 
```java
    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        String userPath=req.getServletPath();
        sessionFactory.getCurrentSession().beginTransaction();
        if ("/user".equals(userPath)){
            int number = EventServlet.getId(req);
            try{
                UserEv user = sessionFactory.getCurrentSession().load(UserEv.class,number);
                sessionFactory.getCurrentSession().remove(user);
                sessionFactory.getCurrentSession().getTransaction().commit();
                req.getRequestDispatcher("/index.jsp").forward(req, resp);
            } catch (Exception e){
                sessionFactory.getCurrentSession().getTransaction().rollback();
                e.printStackTrace();
            }
            sessionFactory.getCurrentSession().close();
        }
    }
```
#### 6. Experience 
* I took a part in EPAM's coding competition "I can code" 
* Also Netcracker's coding competition
* Three course projects at university
#### 7. Education
* **Secondary special education**, Samara college of service technologies and arts, *2012-2016*. 
My specialty is a garment manufacturing technologist
* **High education**, Togliatty State University, *2017-2021*.
My specialty is a applied informatics
* Courses:
  * Coursera online courses "Learning how to learn"
  * JavaRush online courses
  * Basic courses by Mercury Development "QA and QC"
  * Course by Netcracker as a Java developer
#### 8. English 
I had a lot of practice like learning English in school, then in college and university.
I've a confident B1 level and try to improve my skill by learning it by myself, also in university
and I had learning English for 6 months on special courses "Time to Speak".
Also there was a English dictation from Kazan university in September in my univercity , and i won so yesterday I got a diploma
