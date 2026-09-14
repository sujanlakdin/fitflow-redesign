# ADR-001: FitFlow Technology Stack

## Status
Accepted

## Context

FitFlow requires a seamless iOS, Android and web experience with high
performance, AI-powered personalized workouts, camera-based nutrition
tracking, real-time social features, strong security and scalability.

## Decision

The recommended technology stack is:

- Frontend: React Native + React Native Web
- Backend: Node.js + NestJS
- AI Service: Python-based AI service
- AI Model: TensorFlow / TensorFlow Lite
- Computer Vision: ML Kit
- Real-time Data: Firebase Firestore
- Structured Data: PostgreSQL
- Authentication: Firebase Authentication
- Cache: Redis
- Analytics: Firebase Analytics and Mixpanel

## Rationale

React Native provides strong cross-platform code reuse and rapid
development. Node.js/NestJS provides a structured and maintainable
backend. Firestore supports real-time social features. PostgreSQL is
suitable for structured health and workout data. A separate AI service
provides flexibility for AI and computer vision workloads.

## Alternatives Considered

- Flutter
- Kotlin Multiplatform
- Swift/SwiftUI
- Python/FastAPI
- Go
- MongoDB
- DynamoDB
- AWS Cognito
- Auth0
- Supabase

## Consequences

### Positive

- Faster development
- Cross-platform support
- Real-time social features
- Strong AI/ML integration
- Scalable architecture
- Maintainable technology stack

### Negative

- Multiple technologies increase system complexity
- Node.js and Python services require separate maintenance
- Firestore and PostgreSQL require clear data ownership
