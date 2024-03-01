# email_friendcount
Write a SQL query that returns the email address and friend count of the user with the most friends. 

Select
Email,
friend_count
From users 
Where friend_count = (select max(friend_count) from users);
