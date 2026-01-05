# NexOffice

A virtual office platform for remote teams with video calls, screen sharing, and real-time collaboration.

## What It Does

Create virtual office spaces where team members can:
- Join video calls in different rooms
- Share screens and collaborate
- See who's online and in which room
- Navigate between meeting rooms, dev spaces, and creative hubs

## Tech Stack

- **Frontend**: Next.js, TypeScript, Firebase
- **Backend**: FastAPI, WebSockets
- **Video**: WebRTC for peer-to-peer calls

## Quick Start

**Prerequisites**: Node.js 18+, Python 3.9+, Firebase account

1. **Setup Firebase**
   - Create a Firebase project at [console.firebase.google.com](https://console.firebase.google.com/)
   - Enable Google Authentication
   - Create a Firestore database
   - Copy and configure environment variables:
     ```bash
     cd frontend
     cp .env.example .env.local
     # Edit .env.local with your Firebase config
     ```

2. **Run Backend**
   ```bash
   cd backend
   python -m venv .venv
   source .venv/bin/activate  # Windows: .venv\Scripts\activate
   pip install -r requirements.txt
   uvicorn main:app --reload --host 0.0.0.0 --port 8000
   ```

3. **Run Frontend**
   ```bash
   cd frontend
   npm install
   npm run dev
   ```

4. **Open** [localhost:3000](http://localhost:3000)

## Usage

1. Sign in with Google
2. Create or join an office
3. Invite team members
4. Start collaborating

## License

MIT