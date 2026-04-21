# Smart Attendance with Alert Notification System

## Description
A secure web-based attendance management system developed as a Computer Engineering Project at UTeM. 
The system uses dynamic QR codes and GPS verification to prevent proxy attendance, with automated alert notifications to lecturers for at-risk students.

## Problem Statement
Traditional manual attendance is time-consuming and 
vulnerable to proxy attendance (students marking absent 
friends as present). This system solves both problems 
using technology-based verification.

## Features
- Dynamic QR code regeneration every 10 seconds to 
  prevent screenshot abuse and proxy attendance
- GPS validation to verify student is physically present 
  inside the classroom before marking attendance
- Automated alert to lecturer when student misses 
  3 or more classes — triggers warning letter
- Automated bar letter alert when attendance drops 
  below 80%
- Secure login for lecturers and students
- Real-time attendance dashboard

## Tech Stack
| Layer | Technology |
|-------|-----------|
| Frontend | React |
| Backend | Django |
| Database | PostgreSQL |
| Authentication | Django Auth |
| Location | GPS API |
| QR Code | Dynamic QR Generation |

## System Flow
1. Lecturer opens attendance session — QR code generated
2. QR code regenerates every 10 seconds automatically
3. Student scans QR code via mobile
4. GPS verifies student is within classroom boundary
5. Attendance marked only if both QR and GPS verified
6. System tracks cumulative attendance per student
7. Automated alerts sent when thresholds are exceeded

## Alert System
| Condition | Action |
|-----------|--------|
| Miss 3 or more classes | Warning letter issued |
| Attendance below 80% | Bar letter issued |

## Project Info
- **Institution:** Universiti Teknikal Malaysia Melaka (UTeM)
- **Programme:** Bachelor of Computer Engineering with Honours
- **Year:** 2026
- **Supervisor:** Norihan Binti Abdul Hamid
- **Status:** In Progress — completing July 2026
