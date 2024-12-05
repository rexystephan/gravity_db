# postgre
This repository contains the DB details with reference to the script from a public github - https://github.com/bbrumm/databasestar/tree/main/sample_databases/sample_db_gravity/gravity_postgres.
For better self understanding of the above DB, have mentioned the following details.

The DB Gravity has 15 tables in total.
1. address- This table has the
   - columns: Address_id,
              street_number,
              street_name,
              city,
              country_id
   - Constraints : Address_id (primary Key)
                   country_id (Foreign Key - referencing table: country)

2. address_status- This table has the
   - columns: status_id,
              address_status
   - Constraints : status_id (primary Key)    
3. author- This table has the
   columns: author_id,
            author_name
   Constraints : author_id (primary key)
5. 
6. book - This table has the columns: book_id (primary key), title, isbn13, language_id (foreign key - referencing table: book_language), num_pages, publication_date, publisher_id(foreign key - referencing table: publisher)
7. book_author - This table has the columns: book_id (composite primary key), author_id (composite primary key) (foreign key - referencing table: publisher)
    
