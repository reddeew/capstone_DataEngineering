This dataset contains demographic information for each US state.

| Column               | Description                                               |
| -------------------- | --------------------------------------------------------- |
| state_code           | A 2-letter code indicating the US state name.            |
| total_population     | Total population of the state.                           |
| male_population      | Total male population of the state.                      |
| female_population    | Total female population of the state.                    |
| number_of_veterans   | Total number of state veterans.                          |
| foregin_born         | Total number of foreign-born residents.                  |
| median_age           | The average age of the state's population.               |
| average_household_size | Average household size in the state.    


arrival_mode table

 Column           | Description                                                           |
| ---------------- | --------------------------------------------------------------------- |
| arrival_mode_id  | A unique ID representing each arrival mode.                            |
| mode_code        | A code indicating the mode of transport.                               |
| mode             | Description of the code indicating the mode of transport.              |
| airline          | A code consisting of 1 to 3 characters representing the airline code used to arrive in the U.S. |
| flight_number    | A 1- to 5-character code that represents the airline flight number used to arrive in the U.S. |

date table
| Column         | Description                                   |
| -------------- | --------------------------------------------- |
| date           | The date in the format YYYY-MM-DD.           |
| year           | The year component of the date.              |
| quarter        | Quarter number of the year.                  |
| month          | Month number of the year.                    |
| week_of_year   | Week number of the year.                     |
| day_of_week    | Day number of the week (0 - Monday, 6 - Sunday). |
| day_of_month   | Day number of the month.                     |
| day_of_year    | Day number of the year.                      |

status_flag table

| Column          | Description                                     |
| --------------- | ----------------------------------------------- |
| arrival_flag    | 1 character indicating the arrival flag.       |
| departure_flag  | 1 character indicating the departure flag.     |
| update_flag     | 1 character indicating the update flag.        |
| match_flag      | 1 character indicating the match flag.         |

global temparature table

| Column                           | Description                                                         |
| -------------------------------- | ------------------------------------------------------------------- |
| temperature_id                   | A unique ID representing each temperature measurement.              |
| country                          | The name of the country where the temperature measurements were taken. |
| year                             | The year in which the measurements were made.                       |
| month                            | The month in which the measurements were made.                      |
| average_temperature              | Average temperature during the recorded month.                      |
| average_temperature_uncertainty  | Average temperature uncertainty during the recorded month.          |

world airprots table

| Column                | Description                                                                                   |
| --------------------- | --------------------------------------------------------------------------------------------- |
| airport_id            | A code consisting of 3 to 7 characters representing the airport identification code.         |
| airport_name          | Airport name.                                                                                 |
| airport_type          | Indicates the size of the airport (small, medium, or large).                                  |
| iata_code             | A geocode designating many airports and metropolitan areas around the world.                 |
| municipality_code     | A code consisting of 1 to 7 characters representing the identification code of the municipality where the airport is located. |
| municipality          | The name of the municipality where the airport is located.                                   |
| region_code           | A code consisting of 1 to 4 characters representing the identification code of the region of a country where the airport is located. |
| region                | The name of the region in a country where the airport is located.                             |
| country_code          | A 2-character code representing the identification code of the country where the airport is located. |
| country               | The name of the country where the airport is located.                                        |
| continent_code        | A 2-character code representing the identification code of the continent where the airport is located. |
| continent             | The name of the continent where the airport is located.                                     |
| elevation_ft          | The altitude in feet at which the airport is located.                                        |
| latitude              | The latitude of the GPS coordinates.                                                         |
| longitude             | The longitude of the GPS coordinates.     

country temparature evalution

| Column                | Description                                                                                   |
| --------------------- | --------------------------------------------------------------------------------------------- |
| airport_id            | A code consisting of 3 to 7 characters representing the airport identification code.         |
| airport_name          | Airport name.                                                                                 |
| airport_type          | Indicates the size of the airport (small, medium, or large).                                  |
| iata_code             | A geocode designating many airports and metropolitan areas around the world.                 |
| municipality_code     | A code consisting of 1 to 7 characters representing the identification code of the municipality where the airport is located. |
| municipality          | The name of the municipality where the airport is located.                                   |
| region_code           | A code consisting of 1 to 4 characters representing the identification code of the region of a country where the airport is located. |
| region                | The name of the region in a country where the airport is located.                             |
| country_code          | A 2-character code representing the identification code of the country where the airport is located. |
| country               | The name of the country where the airport is located.                                        |
| continent_code        | A 2-character code representing the identification code of the continent where the airport is located. |
| continent             | The name of the continent where the airport is located.                                     |
| elevation_ft          | The altitude in feet at which the airport is located.                                        |
| latitude              | The latitude of the GPS coordinates.                                                         |
| longitude             | The longitude of the GPS coordinates.        


Fact - immigration application table

| Column              | Description                                                           |
| ------------------- | --------------------------------------------------------------------- |
| file_id             | The unique number of the file.                                       |
| ins_number          | INS number.                                                           |
| admission_number    | Admission Number.                                                     |
| applicant_age       | Age of the applicant.                                                 |
| applicant_birth_year | The applicant's year of birth.                                       |
| gender              | Gender of the applicant.                                              |
| occupation          | A 3-character code indicating the occupation the applicant will have in the U.S. |
| visa_id             | The ID that indicates the visa information in the visa table.        |
| application_date    | The date the application was added to the I94 files.                 |
| admission_port_code | Port of admission.                                                    |
| arrival_state_code  | The US state where the applicant arrived.                            |
| arrival_mode_id     | The ID indicating information about how the applicant arrived in the US in the arrival_mode table. |
| arrival_date        | Date of the applicant's arrival to the US.                            |
| departure_date      | Date of the applicant's departure to the US.                          |
| limit_date          | The deadline until which the applicant has the right to stay in the USA. |
| status_flag_id      | The ID indicating information about the status of various flags in the status_flag table. |
| birth_country       | 3-digit code indicating the applicant's country of birth.            |
| residence_country   | 3-digit code indicating the applicant's country of residence.        |

visa table

# Dataset Description

This dataset contains information related to applicants and their admissions to the USA, including visa details and other relevant information.

| Column              | Description                                                           |
| ------------------- | --------------------------------------------------------------------- |
| file_id             | The unique number of the file.                                       |
| ins_number          | INS number.                                                           |
| admission_number    | Admission Number.                                                     |
| applicant_age       | Age of the applicant.                                                 |
| applicant_birth_year | The applicant's year of birth.                                       |
| gender              | Gender of the applicant.                                              |
| occupation          | A 3-character code indicating the occupation the applicant will have in the U.S. |
| visa_id             | The ID that indicates the visa information in the visa table.        |
| application_date    | The date the application was added to the I94 files.                 |
| admission_port_code | Port of admission.                                                    |
| arrival_state_code  | The US state where the applicant arrived.                            |
| arrival_mode_id     | The ID indicating information about how the applicant arrived in the US in the arrival_mode table. |
| arrival_date        | Date of the applicant's arrival to the US.                            |
| departure_date      | Date of the applicant's departure to the US.                          |
| limit_date          | The deadline until which the applicant has the right to stay in the USA. |
| status_flag_id      | The ID indicating information about the status of various flags in the status_flag table. |
| birth_country       | 3-digit code indicating the applicant's country of birth.            |
| residence_country   | 3-digit code indicating the applicant's country of residence.        |

admistion port table

| Column                | Description                                                                                   |
| --------------------- | --------------------------------------------------------------------------------------------- |
| admission_port_code   | A 3-letter code indicating the port of admission.                                            |
| admission_port        | A description of the admission port code indicating information about its location.        |


# US States Dimension Table

This dimension table contains information about US states.

| Column       | Description                                   |
| ------------ | --------------------------------------------- |
| state_code   | A 2-letter code indicating the US state name. |
| state        | US state name.                                |


