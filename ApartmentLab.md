<h3>Apartment Lab Thing</h3>
tim.gray

<hr>

<h6>1</h6>
\dt;

<h6>2</h6>
\du;

<h6>3</h6>
SELECT * FROM owners;

<h6>4</h6>
SELECT name FROM owners;

<h6>5</h6>
SELECT age FROM owners ORDER BY age ASC;                                                                                        

<h6>6</h6>
SELECT name FROM owners WHERE name = 'Donald'

<h6>7</h6>
SELECT age FROM owners WHERE age > 30;

<h6>8</h6>
SELECT * FROM owners WHERE name LIKE 'E%';

<h6>9</h6>
INSERT INTO owners (name,age) VALUES ('John', 33);

<h6>10</h6>
INSERT INTO owners (name,age) VALUES ('Jane', 43);

<h6>11</h6>
UPDATE owners SET age = 30 WHERE name = 'Jane';

<h6>12</h6>
UPDATE owners SET name = 'Janet' WHERE name = 'Jane';

<h6>13</h6>
INSERT INTO properties (name,number_of_units) VALUES ('Archstone', 20);

<h6>14</h6>
DELETE FROM owners WHERE name ='Jane';

<h6>15</h6>
SELECT * FROM properties where name != 'Archstone' AND property_id != 3 AND property_id != 5;

<h6>16</h6>
SELECT COUNT(*) FROM properties;

<h6>17</h6>
SELECT MAX(age) FROM owners;

<h6>18</h6>
SELECT * FROM owners LIMIT 3;

<h6>19</h6>
ALTER TABLE properties ADD CONSTRAINT owner_fk FOREIGN KEY (ownerId) REFERENCES owners (owner_id) ON DELETE NO ACTION;

<h6>20</h6>
SELECT * FROM owners JOIN properties ON owners.owner_id = properties.ownerId;