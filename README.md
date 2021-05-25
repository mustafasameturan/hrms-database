<div align="center"><h1>Human Resources Management System Database Tables</h1> </div>
<div align="center"><h2>İnsan Kaynakları Yönetim Projesi Veritabanı Tabloları</h2> </div>

<div align="center"><h3> 🚩 PostgreSQL programı ve isimlendirme standartları kullanılmıştır. 🚩</h3> </div>

<table>
  <tr>
    <td>users</td>
     <td>job_titles</td>
     <td>employers</td>
  </tr>
  <tr>
    <td>

Variable Name | Data Type
------------ | -------------
id | int
email | varchar(50)
password | varchar(25)
   
   </td>
    <td>

Variable Name | Data Type
------------ | -------------
id | int
title | varchar(50)
   
   </td>
    <td>

Variable Name | Data Type
------------ | -------------
id | int
company_name | varchar(255)
web_address | varchar(50)
phone_number | varchar(12)
is_activated | boolean
   
   </td>
  </tr>
 </table>
 
<table>
  <tr>
     <td>employees</td>
     <td>candidates</td>
     <td>activation_codes</td>
  </tr>
  <tr>
    <td>

Variable Name | Data Type
------------ | -------------
id | int
first_name | varchar(25)
last_name | varchar(25)
   
   </td>
    <td>

Variable Name | Data Type
------------ | -------------
id | int
first_name | varchar(25)
last_name | varchar(25)
identity_number | varchar(11)
birth_date | date
   
   </td>
    <td>

Variable Name | Data Type
------------ | -------------
id | int
activation_code | varchar(38)
is_confirmed | boolean
confirmation_date | date
   
   </td>
  </tr>
 </table>
 
 <table>
  <tr>
     <td>activation_code_to_candidates</td>
     <td>activation_code_to_employers</td>
     <td>employer_activation_by_employees</td>
  </tr>
  <tr>
    <td>

Variable Name | Data Type
------------ | -------------
id | int
candidate_id | int
   
   </td>
    <td>

Variable Name | Data Type
------------ | -------------
id | int
employer_id | int
   
   </td>
    <td>

Variable Name | Data Type
------------ | -------------
id | int
employer_id | int
confirmed_employee_id | int
is_confirmed | boolean
confirmed_date | date    
   
   </td>
  </tr>
 </table>

