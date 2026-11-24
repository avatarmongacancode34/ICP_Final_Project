## Person:
person_id, title, first_name, middle_name, last_name, date_of_birth, gender, nationality, email, phone, street_address, digital_address, city, region, country, emergency_contact_name, emergency_contact_phone, username, password_hash, user_role, account_status

## Student: 
student_id, person_id, program_id, admission_date, expected_graduation_year, academic_level, enrollment_status, previous_school, entry_qualification, guardian_name, guardian_phone, financial_aid_status, cgpa

## Faculty: 
faculty_id, person_id, department_id, academic_rank, specialization, employment_type, employment_date, date_available, years_of_experience, highest_education, university_attended, office_location, employment_status

## Admin: 
admin_id, person_id, department_id, office_or_department, role_or_position, access_level, employment_type, employment_date, employment_status

## Department: 
department_id, department_name, department_code, head_of_department_id, office_location

## Program: 
program_id, department_id, program_name, program_code, degree_type, duration_years, total_credits_required

## Course: 
course_id, department_id, course_code, course_title, credit_hours, description, academic_level, is_active

## Program_Course: 
program_id, course_id, course_type, recommended_semester

## Faculty_Course: 
faculty_id, course_id, semester_id

## Semester: 
semester_id, academic_year, semester_name, start_date, end_date, registration_deadline, is_current

## Enrollment: 
enrollment_id, student_id, course_id, semester_id, enrollment_date, enrollment_status

## Grade: 
grade_id, enrollment_id, faculty_id, continuous_assessment_score, exam_score, total_score, letter_grade, grade_point, date_recorded

## Fee: 
fee_id, student_id, semester_id, fee_type, amount_due, amount_paid, due_date, payment_status

## Payment: 
payment_id, fee_id, admin_id, amount, payment_date, payment_method, receipt_number


