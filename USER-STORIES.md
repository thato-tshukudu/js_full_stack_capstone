# GiftLink User Stories

This document outlines the 8 core user stories for the GiftLink project. These stories should be created as GitHub Issues with their corresponding labels.

---

## User Story 1: User Registration
**Label:** `new`

**As a** new user
**I need** to create an account with email and password
**So that** I can access the GiftLink application

### Details and Assumptions
- Users should provide a valid email address
- Passwords must meet minimum security requirements
- Email verification should be implemented

### Acceptance Criteria
```gherkin
Given I am on the registration page
When I enter a valid email and password
Then my account should be created successfully
And I should receive a confirmation email
And I should be redirected to the login page
```

---

## User Story 2: User Login
**Label:** `new`

**As a** registered user
**I need** to log in with my credentials
**So that** I can access my personalized dashboard

### Details and Assumptions
- Authentication should use JWT tokens
- Session should persist across page refreshes
- Failed login attempts should show error messages

### Acceptance Criteria
```gherkin
Given I am on the login page
When I enter valid credentials
Then I should be authenticated
And I should be redirected to the main dashboard
And my session token should be stored securely
```

---

## User Story 3: Browse Available Gifts
**Label:** `new`

**As a** logged-in user
**I need** to view a list of available gifts
**So that** I can find gifts I'm interested in

### Details and Assumptions
- Gifts should be displayed with images and descriptions
- Pagination should be implemented for large lists
- Filtering options should be available

### Acceptance Criteria
```gherkin
Given I am on the main page
When I view the gifts list
Then I should see all available gifts
And each gift should display name, description, and image
And I should be able to paginate through results
```

---

## User Story 4: Search for Gifts
**Label:** `new`

**As a** logged-in user
**I need** to search for specific gifts by name or category
**So that** I can quickly find what I'm looking for

### Details and Assumptions
- Search should be case-insensitive
- Results should be returned instantly
- Autocomplete suggestions would enhance UX

### Acceptance Criteria
```gherkin
Given I am on the search page
When I enter a search query
Then relevant gifts should be displayed
And results should be sorted by relevance
And search should handle empty results gracefully
```

---

## User Story 5: View Gift Details
**Label:** `new`

**As a** logged-in user
**I need** to view detailed information about a specific gift
**So that** I can make informed decisions about gifts

### Details and Assumptions
- Details should include full description, price, and availability
- User reviews and ratings should be displayed
- Similar gift recommendations should be shown

### Acceptance Criteria
```gherkin
Given I click on a gift item
When the details page loads
Then I should see complete gift information
And I should see user reviews and ratings
And I should see related product recommendations
```

---

## User Story 6: Sentiment Analysis on Reviews
**Label:** `technical debt`

**As a** developer
**I need** to implement sentiment analysis on user reviews
**So that** we can categorize and rank reviews by sentiment

### Details and Assumptions
- Use existing sentiment analysis module
- Analyze review text for positive, negative, and neutral sentiment
- Cache results to improve performance

### Acceptance Criteria
```gherkin
Given a user review is submitted
When the review is processed
Then sentiment analysis should be performed
And sentiment score should be stored
And reviews should be sorted by sentiment in UI
```

---

## User Story 7: User Profile Management
**Label:** `backlog`

**As a** logged-in user
**I need** to update my profile information
**So that** my account details remain current and accurate

### Details and Assumptions
- Users should be able to update name, email, and preferences
- Profile picture upload should be supported
- Password change functionality should be available

### Acceptance Criteria
```gherkin
Given I am on my profile page
When I update my information
Then changes should be saved to the database
And I should receive a confirmation message
And updates should be reflected immediately
```

---

## User Story 8: Wishlist Management
**Label:** `icebox`

**As a** logged-in user
**I need** to add gifts to my wishlist
**So that** I can save items for future reference

### Details and Assumptions
- Users should be able to create multiple wishlists
- Wishlists should be shareable via link
- Wishlist items should be organized by priority

### Acceptance Criteria
```gherkin
Given I am viewing a gift
When I click "Add to Wishlist"
Then the gift should be saved to my wishlist
And I should see a confirmation message
And the item should appear in my wishlist page
```

---

## How to Create These Issues in GitHub

1. Go to your repository: https://github.com/thato-tshukudu/js_full_stack_capstone
2. Click on "Issues" tab
3. Click "New Issue"
4. Select "User Story" from the template dropdown
5. Fill in the story details from this document
6. Apply the corresponding label (new, icebox, technical debt, backlog)
7. Repeat for each of the 8 user stories above
