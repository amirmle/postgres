# CREATE TABLE

    CREATE TABLE cars (
      brand VARCHAR(255),
      model VARCHAR(255),
      year INT
    );



# Insert 

    INSERT INTO cars (brand, model, year)
    VALUES ('Ford', 'Mustang', 1964);
    
    INSERT INTO cars (brand, model, year)
    VALUES
      ('Volvo', 'p1800', 1968),
      ('BMW', 'M1', 1978),
      ('Toyota', 'Celica', 1975);

# Select

    SELECT * FROM cars;
    SELECT brand, year FROM cars;

# ADD COLUMN

    ALTER TABLE cars
    ADD color VARCHAR(255);

# UPDATE

    UPDATE cars
    SET color = 'red'
    WHERE brand = 'Volvo';

    UPDATE cars
    SET color = 'white', year = 1970
    WHERE brand = 'Toyota';

# ALTER COLUMN

    ALTER TABLE cars
    ALTER COLUMN year TYPE VARCHAR(4);

# DROP COLUMN

    ALTER TABLE cars
    DROP COLUMN color;


# DELETE 

    DELETE FROM cars
    WHERE brand = 'Volvo';

    DELETE FROM cars;

- also deletes all records

        TRUNCATE TABLE cars;


# DROP TABLE
    
    DROP TABLE cars;
