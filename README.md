# URL-Shortner
A role-based URL Shortener built using .Users belong to companies and have different permissions based on roles (Admin, Member, Sales, Manager).
URL Shortener Service (Laravel 10–12)

This project is a role-based URL Shortener system developed as part of the Sembark Tech Backend Developer Assignment.
Users belong to companies and have specific role-based permissions for invitations and URL operations.

Features -
Authentication & Authorization

Laravel Breeze authentication (login/register/logout)

Role-based access control using custom middleware

Roles supported -
SuperAdmin, Admin, Member, Sales, Manager

 Company Management

Each user belongs to one company

SuperAdmin does not belong to any company

Invitation rules enforced

URL Shortener

Sales & Manager can create short URLs

Short URLs redirect to original URLs (after authentication)

URLs are not publicly resolvable

Listing rules - 

Admin: Can see URLs not created in their own company

Member: Can see URLs not created by themselves

SuperAdmin: Cannot see all URLs

Tests (Manually Verified)

Unauthorized roles cannot create URLs

Listing filters based on role rules

Short URLs require authentication to access
