# Interview Scheduling System API Gateway with Docker, PostgreSQL, NestJS, and Typeform Integration
Develop an API gateway for a corporate interview scheduling system employing Docker, PostgreSQL, NestJS, and Typeform integration. 

Here are the key functionalities:

1. **User Authentication**:
   - Allow interviewers to sign in and sign up.
   
2. **Interview Creation**:
   - Interviewers can create interviews.

3. **Available Slot Management**:
   - After creating an interview, interviewers can add available slots for the interview.
   - Each slot must be unique and not available for booking by multiple candidates simultaneously.
   
4. **Unique Interview Links**:
   - Generate a unique interview link for each interview, which can be shared with all candidates.
   
5. **Candidate Booking**:
   - Candidates can access the interview link and select a suitable slot.
   - To book a slot, candidates must provide their email address and name.
   - Once a slot is booked by one candidate, it should be unavailable for other candidates.

To accomplish this, you'll need to:

- **Database Design**: Define the database schema for storing interviewers, interviews, available slots, candidates, and their bookings.

- **API Endpoints**:
   - Implement API endpoints for user authentication, interview creation, slot management, and candidate bookings.
   - Handle slot availability and booking logic within these endpoints.
   - Create an endpoint to generate unique interview links.

- **Integration with Typeform**: Integrate Typeform for generating and sharing unique interview links.

- **Testing**:
   - Develop test cases to ensure the system functions correctly.
   - Include unit tests, integration tests, and end-to-end tests as needed.
   - Verify that slot booking logic works as expected, and candidates cannot double-book slots.

Sample API endpoints might include:

- `/auth/signup` and `/auth/signin` for user authentication.
- `/interviews/create` to create interviews.
- `/interviews/:id/slots/add` to add available slots to an interview.
- `/interviews/:id/candidates/book` to allow candidates to book slots.
- `/interviews/:id/unique-link` to generate a unique interview link for sharing.

Remember to follow best practices in NestJS, use Docker for containerization, and ensure proper PostgreSQL database setup. Test your system thoroughly to guarantee reliability and correctness.

## Submitting Your Work
1. Create a new repository on GitHub and add the original files
2. Add `ijazulrehman` as repository collaborators 

