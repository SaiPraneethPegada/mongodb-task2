 **Create DB:**
 
    use Zen_Class

**1. Mentors Collection creation and Data Insert:**

> db.createCollection('mentors');

    db.mentors.insertMany([
        {
            mentorid: 1,
            mentorname: "mentor1",
            mentor_email: "mentor1@gmail.com",
        },
        {
            mentorid: 2,
            mentorname: "mentor2",
            mentor_email: "mentor2@gmail.com",
        },
        {
            mentorid: 3,
            mentorname: "mentor3",
            mentor_email: "mentor3@gmail.com",
        },
        {
            mentorid: 4,
            mentorname: "mentor4",
            mentor_email: "mentor4@gmail.com",
        },
        {
            mentorid: 5,
            mentorname: "mentor5",
            mentor_email: "mentor5@gmail.com",
        },
    ]);


**2. Users Collection creation and Data Insert:**

> db.createCollection("users");

    db.users.insertMany([
        {
            userid:1,
            name:"user1",
            email:"user1@gmail.com",
            mentorid:1,
        },
        {
            userid:2,
            name:"user2",
            email:"user2@gmail.com",
            mentorid:1,
        },
        {
            userid:3,
            name:"user3",
            email:"user3@gmail.com",  
            mentorid:2,
        },
        {
            userid:4,
            name:"user4",
            email:"user4@gmail.com",
            mentorid:3,
        },
        {
            userid:5,
            name:"user5",
            email:"user5@gmail.com",
            mentorid:5,
        }
    ]);


**3. codekata Collection creation and Data Insert:**
 
 > db.createCollection('codekata');

    db.codekata.insertMany([
        {
            codekata_id :1,
            category: "Input/Output",
            problems: 10,
        },
        {
            codekata_id :2,
            category: "Absolute Beginner",
            problems: 30,
        },
        {
            codekata_id :3,
            category: "Array",
            problems: 300,
        },
        {
            codekata_id :4,
            category: "Strings",
            problems: 200,
        },
        {
            codekata_id :5,
            category: "Basics",
            problems: 40,
        }
    ]);


**4. Topics Collection creation and Data Insert:**

> db.createCollection('topics');

    db.topics.insertMany([
        {
            topicid: 1,
            topic: "html",
            topic_date: new Date("1-sep-2022"),
        },
        {
            topicid: 2,
            topic: "css",
            topic_date: new Date("5-sep-2022"),
        },
        {
            topicid: 3,
            topic: "Javascript",
            topic_date: new Date("10-sep-2022"),
        },
        {
            topicid: 4,
            topic: "React",
            topic_date: new Date("20-sep-2022"),
        },
        {
            topicid: 5,
            topic: "NodeJs",
            topic_date: new Date("30-sep-2022"),
        },
    ]);


**5. Tasks Collection creation and Data Insert:**

> db.createCollection('tasks');

    db.tasks.insertMany([
        {
            taskid: 1,
            topicid: 1,
            userid: 1,
            task: "html task",
            due_date: new Date("4-oct-2021"),
            submitted: true,
        },
        {
            taskid: 2,
            topicid: 2,
            userid: 2,
            task: "css task",
            due_date: new Date("10-oct-2021"),
            submitted: true,
        },
        {
            taskid: 3,
            topicid: 3,
            userid: 3,
            task: "Javascript task",
            due_date: new Date("15-oct-2021"),
            submitted: false,
        },
        {
            taskid: 4,
            topicid: 4,
            userid: 4,
            task: "React task",
            due_date: new Date("20-oct-2021"),
            submitted: false,
        },
        {
            taskid: 5,
            topicid: 5,
            userid: 5,
            task: "Node task",
            due_date: new Date("25-oct-2021"),
            submitted: false,
        },
    ]);


**6. Attendance Collection creation and Data Insert:**

> db.createCollection('attendance');

    db.attendance.insertMany([
        {
            userid: 1,
            topicid: 1,
            attended: true,
        },
        {
            userid: 1,
            topicid: 2,
            attended: true,
        },
        {
            userid: 1,
            topicid: 3,
            attended: false,
        },
        {
            userid: 2,
            topicid: 3,
            attended: false,
        },
        {
            userid: 5,
            topicid: 5,
            attended: false,
        },
    ]);


**7. companydrives collection creation and Data Insert:**

> db.createCollection('companydrives');

    db.companydrives.insertMany([
        {
            userid: 1,
            drive_date: new Date("10-nov-2022"),
            company: "Google",
            selection: false,
        },
        {
            userid: 1,
            drive_date: new Date("15-nov-2022"),
            company: "Amazon",
            selection: false,
        },
        {
            userid: 2,
            drive_date: new Date("20-nov-2022"),
            company: "Google",
            selection: true,
        },
        {
            userid: 3,
            drive_date: new Date("25-nov-2022"),
            company: "TCS",
            selection: true,
        },
        {
            userid: 4,
            drive_date: new Date("27-nov-2022"),
            company: "Wipro",
            selection: true,
        },
    ]);
