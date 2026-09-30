# RBIS Learning Platform

Student mobile application for tests, olympiads, and educational monitoring.

## 📁 Documentation

- **[Mobile UI/TZ Specification](docs/rbis-mobile-ui-spec.md)** — Complete product and design specification for Figma/AI

## 🎨 Brand identity

**Primary color (burgundy):**
- HEX: #5f0521
- RGB: 95, 5, 33
- CMYK: 36%, 100%, 71%, 54%

**Secondary colors:**
- Black: #090909
- White: #F7F7F7
- Success: #2FAE66
- Error: #D94A5D
- Warning: #F2B84B

## 🎯 Product scope

**Student app features:**
- User onboarding and authentication (phone, Google, Telegram)
- Subject-based test library
- Open, closed, topic-based, and olympiad tests
- Real-time performance monitoring and analytics
- Leaderboard and achievement system
- Certificates and badges
- Push notifications
- Profile and settings

## 🚀 Tech stack

- Target platforms: iOS, Android
- Recommended framework: Flutter, React Native, or native
- Backend: Node.js / Python / Go
- Database: PostgreSQL / MongoDB
- Real-time: WebSocket for olympiad events

## 📋 MVP scope

1. Auth (phone, Google, Telegram)
2. Subject selection
3. Test list and filtering
4. Test flow with autosave and timer
5. Results and review
6. Olympiad registration and synchronized start
7. Leaderboard
8. Push notifications
9. Profile with stats

## 🔒 Security requirements

- Server-based time validation
- App switch detection
- Screenshot blocking (Android FLAG_SECURE)
- One session per device per account
- No answer leakage before submission

## 📱 UI/UX design

All screen designs are detailed in the specification document.
Recommended workflow:
1. Import specification into Figma
2. Use AI to generate first-pass screens
3. Refine with brand guidelines
4. Prepare for development handoff

---

**Version:** 1.0  
**Last updated:** September 30, 2026  
**Status:** Ready for design phase
