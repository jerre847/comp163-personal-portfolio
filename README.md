# comp163-personal-portfolio
# Personal / Academic Info
full_name = "Jeremiah Young"
student_email = "jdyoung7@ncat.edu"
hometown = "Charlotte, NC"
graduation = "Spring 2029"
major = "Electrical engineering"

# Academic Profile
current_semester_credits = 13
current_courses = [
    {"code": "COMP 163", "credits": 3, "instructor": "Prof. Rhodes", "location": "M-Eric 300"},
    {"code": "MATH 150", "credits": 3, "instructor": "Dr. Lee", "location": "Marteena 201"},
    {"code": "ENG 101", "credits": 3, "instructor": "Dr. Martinez", "location": "Crosby 121"},
    {"code": "HIS 105", "credits": 3, "instructor": "Dr. Brown", "location": "Crosby 210"}
]
cumulative_gpa = 3.87
weekly_study_hours = 22
academic_investment_per_hour = 4.0

# Personal Development
current_skills = ["Time management", "Photography", "Problem solving", "HTML", "Python basics"]
learning_goals = ["Data structures", "Web design", "JavaScript", "Git", "Public speaking"]
career_interests = ["Software development", "Game development", "Web development", "Data science"]

# Financial Overview
monthly_budget = 875
budget_breakdown = {
    "Food": 550,          # $ per month
    "Entertainment": 1000,
    "Books": 129,
    "Transportation": 200
}
daily_food_estimate = 17.0
annual_projection = 10600

# Connections & Contacts
emergency_contact_name = "Hannah Smith (Mom)"
emergency_contact_phone = "704-655-0189"
home_address = "456 Oak Street, Charlotte, NC 28202"
social_media_followers = 1,497
social_platforms = 3
key_contacts = 4

# Life Statistics
total_courses_completed = 5
current_academic_load = 37
entertainment_backlog = 5
current_hobbies = 5

# Helper: pretty-print a section header
def print_header(title):
    print("=" * 60)
    print(title)
    print("=" * 60)

# Output the formatted portfolio
def print_portfolio():
    print("====")
    print("=" * 60)
    print("PERSONAL ACADEMIC & LIFE PORTFOLIO")
    print("====")
    print("=" * 60)
    print(f"Student: {full_name} | Email: {student_email}")
    print(f"From: {hometown} | Graduating: {graduation}")
    print(f"Major: {major}")
    print("===")
    print("ACADEMIC PROFILE")
    print("===")
    print(f"Current Semester: {current_semester_credits} credits across {len(current_courses)} courses")
    print(f"Cumulative GPA: {cumulative_gpa}")
    print(f"Weekly Study Time: {weekly_study_hours} hours")
    print(f"Academic Investment: ${academic_investment_per_hour:.1f} per study hour")
    print("Current Courses:")
    for c in current_courses:
        print(f"{c['code']} - {c['credits']} credits - {c['instructor']} - {c['location']}")
    print("===")
    print("PERSONAL DEVELOPMENT")
    print("===")
    print(f"Current Skills: {current_skills}")
    print(f"Learning Goals: {learning_goals}")
    print(f"Career Interests: {career_interests}")
    print(f"Skills Currently Have: {len(current_skills)}")
    print(f"Skills Want to Learn: {len(learning_goals)}")
    print("===")
    print("FINANCIAL OVERVIEW")
    print("===")
    print(f"Monthly Budget: ${monthly_budget}")
    for k, v in budget_breakdown.items():
        if k == "Food":
            print(f"{k}: ${v} (${daily_food_estimate}/day)")
        else:
            print(f"{k}: ${v}")
    print(f"Annual Projection: ${annual_projection}")
    print("===")
    print("CONNECTIONS & CONTACTS")
    print("===")
    print(f"Emergency Contact: {emergency_contact_name} - {emergency_contact_phone}")
    print(f"Home Address: {home_address}")
    print(f"Social Media Presence: {social_media_followers} followers across {social_platforms} platforms")
    print(f"Key Contacts: {key_contacts} people in directory")
    print("===")
    print("LIFE STATISTICS")
    print("===")
    print(f"Total Courses Completed: {total_courses_completed}")
    print(f"Current Academic Load: {current_academic_load} weekly commitments")
    print(f"Entertainment Backlog: {entertainment_backlog} items")
    print(f"Current Hobbies: {current_hobbies} activities")
    print("====")
    print("=" * 35)

# Run the display function (safe for ZyBooks)
if __name__ == "__main__":
    print_portfolio()
