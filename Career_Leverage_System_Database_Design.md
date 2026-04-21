# Career Leverage System Database Design Document

## Overview
This document outlines the design for a Career Leverage System focused on policy professionals. It details the structure of 7 interconnected databases, their properties, relationships, formulas, views, and implementation guidance.

### Databases Overview
1. **User Profiles**  
   - **Properties:**  
     - User ID (Primary Key)  
     - Name  
     - Email  
     - Phone Number  
     - LinkedIn Profile  
   - **Relationships:**  
     - One-to-Many with Career Goals  
     - One-to-Many with Skills

2. **Career Goals**  
   - **Properties:**  
     - Goal ID (Primary Key)  
     - User ID (Foreign Key)  
     - Goal Description  
     - Target Date  
     - Status  
   - **Relationships:**  
     - Many-to-One with User Profiles
     - Many-to-Many with Professional Opportunities

3. **Skills**  
   - **Properties:**  
     - Skill ID (Primary Key)  
     - User ID (Foreign Key)  
     - Skill Name  
     - Proficiency Level  
   - **Relationships:**  
     - Many-to-One with User Profiles  
     - Many-to-Many with Training Courses

4. **Professional Opportunities**  
   - **Properties:**  
     - Opportunity ID (Primary Key)  
     - Title  
     - Description  
     - Company  
     - Location  
   - **Relationships:**  
     - Many-to-Many with Career Goals

5. **Training Courses**  
   - **Properties:**  
     - Course ID (Primary Key)  
     - Course Name  
     - Provider  
     - Duration  
     - Cost  
   - **Relationships:**  
     - Many-to-Many with Skills

6. **Networking Contacts**  
   - **Properties:**  
     - Contact ID (Primary Key)  
     - User ID (Foreign Key)  
     - Name  
     - Email  
     - Relationship Type  
   - **Relationships:**  
     - Many-to-One with User Profiles

7. **Job Applications**  
   - **Properties:**  
     - Application ID (Primary Key)  
     - User ID (Foreign Key)  
     - Opportunity ID (Foreign Key)  
     - Application Date  
     - Status  
   - **Relationships:**  
     - Many-to-One with User Profiles  
     - Many-to-One with Professional Opportunities

## Formulas
- **Skill Proficiency Score:**
  - Calculation of an average score from multiple training courses and assessments.

## Views
- **User Dashboard:**
  - Overview of career goals, skills, and applications status.

## Implementation Guidance
1. **Database Setup:**  
   - Use a relational database management system (RDBMS) for optimal interconnectivity.
   - Ensure normalization to minimize redundancy and maintain data integrity.
2. **Data Entry:**  
   - Implement forms for easy input of user profiles, skills, and goals.
   - Integrate APIs for pulling in professional opportunities.
3. **Regular Updates:**  
   - Schedule routine reviews of data entries for accuracy.

---  
This Career Leverage System is designed to aid policy professionals in managing their careers effectively through interconnected database structures and efficient data management practices.