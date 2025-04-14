# Earnly - Learn & Earn Blockchain Rewards

## Project Title
Earnly - A Blockchain Learning Platform For Learning and Earning

## Selected Domain
Educational Technology (EdTech) with Blockchain Integration

## Problem Statement / Use Case
Traditional educational platforms often struggle with student engagement and lack clear incentive structures. Meanwhile, blockchain technology remains inaccessible to many due to complex learning curves and technical barriers. Earnly addresses these problems by creating a blockchain education platform that rewards learners with cryptocurrency tokens as they progress through courses, thereby solving two issues simultaneously:

1. Increasing student engagement and motivation in online learning through gamification and reward mechanisms
2. Lowering the barrier to entry for blockchain technology by providing accessible education with practical token rewards

## Abstract / Problem Description
Earnly is a gamified learning platform focused on blockchain education that rewards users with cryptocurrency tokens as they progress through courses. It combines educational content with real-world incentives, creating a self-reinforcing ecosystem where learning leads to tangible rewards.

The current e-learning landscape faces significant challenges with student retention and engagement. Many platforms struggle to keep users motivated throughout the learning journey, resulting in high dropout rates. Additionally, while blockchain technology adoption continues to grow, there remains a significant knowledge gap that prevents wider acceptance and utilization.

Earnly's "learn-to-earn" model addresses these issues by integrating educational content with blockchain technology. Learners progress through structured courses on blockchain fundamentals, smart contracts, Web3 development, and related topics. As they complete modules, quizzes, and practical exercises, they earn cryptocurrency tokens that provide immediate value and practical experience with the very technology they're learning about.

The platform features a comprehensive dashboard that tracks progress, displays earned rewards, shows course recommendations, and enables social learning through leaderboards. This approach creates multiple motivational drivers: the intrinsic value of education, the extrinsic value of token rewards, and the social aspect of community recognition and competition.



## Tech Stack Used
- **Frontend**: HTML5, CSS3, JavaScript (ES6+), Bootstrap 5
- **UI Components**: Bootstrap modals, cards, responsive grid system
- **Animation/Effects**: AOS (Animate On Scroll) library
- **Icons**: Font Awesome
- **Data Visualization**: Chart.js
- **Backend**: Node.js, Express.js
- **Database**: MongoDB (implied by models structure)
- **API Integration**: RESTful API architecture
- **Authentication**: JWT (JSON Web Token) based authentication
- **Storage**: Browser LocalStorage for client-side persistence
- **Blockchain Integration**: Aptos blockchain for token-based reward system (APT tokens)


## Project Structure
The project is organized into the following key directories:
- `public/`: Frontend static files (HTML, CSS, JavaScript)
- `models/`: Database models and schemas
- `routes/`: API route handlers
- `aptos-reward-backend/`: Blockchain integration for token rewards
- `scripts/`: Utility scripts
- `server.js`: Main application entry point
- Seed files for populating the database with initial data

## Project Explanation

### Core Features

#### 1. User Management
- Secure authentication system with login/signup functionality
- Comprehensive user profiles with customizable information
- Profile editing capabilities including photo uploads

![image](https://github.com/user-attachments/assets/9be0c38a-cc8a-49c7-b17d-e9ed3f743d64)

![image](https://github.com/user-attachments/assets/fa6317f7-504f-42e9-9e5b-e23ac9a10278)

#### 2. Course Management
- Catalog of blockchain-focused courses with filtering capabilities
- Course details pages with progress tracking
- Module-based learning structure with different content types (video, text, quiz)

![image](https://github.com/user-attachments/assets/bcc96ec7-c259-4f08-b412-15c39b456667)

![image](https://github.com/user-attachments/assets/7862cf12-0eac-4c20-b561-febef8809e26)

#### 3. Gamification Elements
- Token rewards for completing courses and modules
- Progress tracking with visual indicators
- Leaderboards to promote healthy competition

![image](https://github.com/user-attachments/assets/67182a6a-006b-47c0-ac74-4af6aeaf314c)


#### 4. Wallet Integration
- Native wallet functionality to store earned tokens
- Transaction history for viewing reward earnings
- Amount will be directly added to petra Wallet

![image](https://github.com/user-attachments/assets/bc46fe72-fc86-48b1-a7a0-410fe431fbbf)

![image](https://github.com/user-attachments/assets/9dfc905d-a86b-409d-9987-af3da16bec61)


#### 5. Dashboard
- Personalized dashboard showing enrolled courses
- Progress statistics and activity feed
- Earnings summary and certificates earned

![image](https://github.com/user-attachments/assets/8c0c4340-e265-4fd4-b2a3-cededfc59aff)

#### 6. Admin Panel
The platform includes a comprehensive admin panel for platform management with the following features:

- **Admin Dashboard**
  - Real-time analytics showing user growth, activity, and engagement metrics
  - Key statistics including total users, courses, quizzes, and token distributions
  - Visual charts for user acquisition and platform activity
  - Recent user activity monitoring
 
    ![image](https://github.com/user-attachments/assets/d26f3921-139c-4772-bc47-c45438fd9e17)


- **User Management System**
  - Complete user database with search and filter functionality
  - User profile editing and wallet balance management
  - User activity tracking and course enrollment monitoring
  - Role-based access control (admin vs regular users)
 
![image](https://github.com/user-attachments/assets/c6c70681-f25a-4cc6-a82f-bca474760056)


- **Course Management**
  - Course creation and editing interface
  - Module builder with support for different content types
  - Ability to set reward amounts for course completion
  - Course statistics including enrollment and completion rates
 
    ![image](https://github.com/user-attachments/assets/0979a207-c7ea-4a74-98ec-5f4ed12728f9)

- **Quiz Management**
  - Comprehensive quiz builder with multiple question types
  - Quiz settings including time limits and passing scores
  - Reward configuration for quiz completion
  - Performance analytics for questions and completion rates
 
    ![image](https://github.com/user-attachments/assets/7b0267c9-8887-4097-b05d-4d255b6549f7)


- **Transaction Monitoring**
  - Complete transaction history across the platform
  - Filtering by transaction type, date, and user
  - Visual representation of token distribution over time
  - Transaction details with status tracking

![image](https://github.com/user-attachments/assets/c8d153f4-d8d4-41ea-bc69-79b2464670f3)

#### 7. AI-Powered Assistance
- **Interactive Chatbot**
  - Real-time assistance on platform features and blockchain concepts
  - Personalized responses based on user's learning progress and token balance
  - Provides instant answers about earning tokens, course information, and technical support
  - Accessible from all pages through a floating chat interface

![image](https://github.com/user-attachments/assets/e5f44671-7142-4d13-a18b-33513d15c4ed)

- **AI Call Assistant**
  - Voice-based assistance for more complex inquiries
  - Connects users with an AI assistant capable of explaining blockchain concepts
  - Helps troubleshoot platform issues in real-time
  - Available through the "Call Assistance" navigation link

![image](https://github.com/user-attachments/assets/67d42bef-e4a3-4de1-90bd-ad1e80176902)

### Architecture & Implementation

The application follows a modular architecture with separate components for:

1. **Authentication**: Handled through the auth.js file, with JWT tokens stored in localStorage
2. **Navigation**: Dynamic navigation loading based on user authentication state
3. **Course Display**: Courses are loaded dynamically from the backend API
4. **User Dashboard**: Comprehensive view of user data, course progress, and rewards
5. **Profile Management**: Complete profile editing capabilities with real-time updates
6. **Backend API**: Express.js routes handle data operations and user interactions
7. **Blockchain Integration**: Aptos blockchain integration for managing token rewards

![Architecture Diagram](https://via.placeholder.com/800x500?text=Application+Architecture)

The frontend communicates with a backend API that manages user data, course content, progress tracking, and token rewards. The system uses RESTful endpoints for data exchange and JWT tokens for secure authentication.

### User Flow

1. Users register or log in to access the platform
2. From the dashboard, users can browse available courses
3. After enrolling, users progress through course modules in sequence
4. Upon completing modules or entire courses, users automatically earn token rewards
5. Progress and earnings are tracked on the dashboard
6. Users can participate in the community through leaderboards and eventually games

![User Flow](https://via.placeholder.com/800x400?text=User+Flow+Diagram)

### User Interface Highlights

#### Home Page
![Home Page](https://via.placeholder.com/600x300?text=Home+Page)

#### Course Listing
![Course Listing](https://via.placeholder.com/600x300?text=Course+Listing)

#### Course Details
![Course Details](https://via.placeholder.com/600x300?text=Course+Details)

#### Learning Interface
![Learning Interface](https://via.placeholder.com/600x300?text=Learning+Interface)

#### Quiz Experience
![Quiz Experience](https://via.placeholder.com/600x300?text=Quiz+Experience)

#### Rewards Celebration
![Rewards Celebration](https://via.placeholder.com/600x300?text=Rewards+Celebration)

### Setup and Installation

1. Clone the repository:
```bash
git clone https://github.com/ABHI10092004/Earnly-Learn-easy-Earn-easy.git
```

2. Install dependencies:
```bash
cd Earnly-Learn-easy-Earn-easy
npm install
```

3. Configure environment variables in `.env` file

4. Seed the database with initial data:
```bash
node run-seed.js
node seed-admin.js
node seed-leaderboard.js
node seed-quizzes.js
```

5. Start the server:
```bash
node server.js
```

### Future Enhancements

- Mobile application development
- Expanded course catalog beyond blockchain topics
- NFT certificates for course completion
- Peer-to-peer learning and mentoring
- Integration with major blockchain networks for wider token utility
- Creator marketplace for user-generated educational content

![Future Roadmap](https://via.placeholder.com/800x400?text=Future+Roadmap)

## Repository

The project is available on GitHub: [Earnly-Learn-easy-Earn-easy](https://github.com/ABHI10092004/Earnly-Learn-easy-Earn-easy.git)
