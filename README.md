# ChatFluent

ChatFluent is a modern web application designed to connect language learners for real-time chat and video calls. It allows users to find language exchange partners, send friend requests, and communicate via text and video in a seamless, interactive interface.

## Features

- **User Authentication:** Secure sign-up, login, logout, and onboarding process.
- **Profile Matching:** Discover recommended language partners based on your learning and native languages.
- **Friend System:** Send, accept, and manage friend requests.
- **Real-Time Chat:** 1:1 messaging with your friends using [Stream Chat](https://getstream.io/chat/).
- **Video Calling:** Instantly start video calls with your contacts (powered by [Stream Video](https://getstream.io/video/)).
- **Notifications:** Stay updated on friend requests and messages.
- **Theming:** Switch between light/dark modes for a personalized experience.

## Tech Stack

- **Frontend:** React, React Router, [stream-chat-react](https://github.com/GetStream/stream-chat-react), [@stream-io/video-react-sdk](https://github.com/GetStream/stream-video-js)
- **Backend:** Node.js, Express, MongoDB (with Mongoose)
- **APIs:** Stream Chat & Video APIs
- **State Management:** React Query
- **Styling:** CSS, Tailwind CSS (or similar utility framework)

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- MongoDB database
- [GetStream account](https://getstream.io/) (for chat and video functionality)
- Yarn or npm

### Setup

#### 1. Clone the repository

```bash
git clone https://github.com/pushkar-2004/ChatFluent.git
cd ChatFluent
```

#### 2. Install dependencies

```bash
cd backend
npm install
cd ../frontend
npm install
```

#### 3. Environment variables

Create `.env` files in both `backend` and `frontend` folders.

**Backend (.env):**
```
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
STREAM_API_KEY=your_stream_api_key
STREAM_API_SECRET=your_stream_api_secret
```

**Frontend (.env):**
```
VITE_STREAM_API_KEY=your_stream_api_key
```

#### 4. Run the backend server

```bash
cd backend
npm run dev
```

#### 5. Run the frontend

```bash
cd frontend
npm run dev
```

The frontend will usually be available at `http://localhost:5173` and backend at `http://localhost:5000`.

## Usage

1. Sign up and complete your onboarding (set your native and learning languages).
2. Find recommended partners and send friend requests.
3. Chat or start a video call with your friends.

## Project Structure

```
ChatFluent/
├── backend/            # Node.js Express API
│   ├── src/
│   └── ...
├── frontend/           # React app
│   ├── src/
│   └── ...
└── README.md
```

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

## License

This project does not currently specify a license.

---

> **Note:** You will need valid Stream Chat and Video credentials to use all features.
