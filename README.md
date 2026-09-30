-- Week 5 Database Assignment Answers

-- Question 1: Drop index IdxPhone from customers table
DROP INDEX IdxPhone ON customers;


-- Question 2: Create user bob with specified password restricted to localhost
CREATE USER 'bob'@'localhost' IDENTIFIED BY '_$S$cu3r3!_';


-- Question 3: Grant INSERT privilege on salesDB database to bob
GRANT INSERT ON salesDB.* TO 'bob'@'localhost';
FLUSH PRIVILEGES;


-- Question 4: Change password for user bob
ALTER USER 'bob'@'localhost' IDENTIFIED BY '_$P$55!23_';
FLUSH PRIVILEGES;
