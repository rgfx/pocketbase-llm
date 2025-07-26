# PocketBase Complete Distilled Reference

> A comprehensive, developer-friendly reference guide for PocketBase - the open source backend in 1 file.

## 🎯 What is This?

This is a distilled, complete reference for **PocketBase** - covering everything from basic setup to advanced server-side extensions. Think of it as your go-to cheat sheet and learning resource for building applications with PocketBase.

**PocketBase** is an open source backend consisting of:
- Embedded database (SQLite) with realtime subscriptions
- Built-in authentication management  
- Convenient dashboard UI
- Simple REST-ish API
- Can be used as both Go framework and standalone application

## 📚 What's Included

### Core Topics Covered
- **🚀 Quick Start** - Get up and running in minutes
- **🏗️ Core Concepts** - Collections, API Rules, Security
- **💻 Client-Side Integration** - Complete JavaScript SDK usage
- **🔐 Authentication** - Password, OAuth2, OTP, Multi-Factor Auth
- **📊 CRUD Operations** - Create, Read, Update, Delete with examples
- **📁 File Management** - Upload, URLs, protected files
- **⚡ Realtime Subscriptions** - Live data updates
- **🔧 Server-Side Extension** - JavaScript hooks and custom routes
- **👑 Admin API** - Collection and settings management
- **🎛️ Advanced Features** - Field types, migrations, deployment
- **✅ Best Practices** - Security, performance, common patterns
- **🐛 Troubleshooting** - Common issues and solutions

### Code Examples For
```javascript
// Authentication
await pb.collection('users').authWithPassword('user@example.com', 'password');

// CRUD Operations  
const record = await pb.collection('posts').create({title: 'Hello World'});

// Realtime Subscriptions
pb.collection('posts').subscribe('*', (e) => console.log(e.action, e.record));

// Server-side Hooks
onRecordAfterCreateRequest((e) => {
    // Send welcome email
    e.next();
}, "users");
```

## 🎯 Who This Is For

- **Frontend Developers** building SPAs, mobile apps, or desktop applications
- **Full-stack Developers** who want a simple, powerful backend solution
- **Backend Developers** looking to extend PocketBase with custom logic
- **Students & Beginners** learning modern backend development
- **Experienced Developers** who need a quick reference while coding

## 🚀 Getting Started

### Option 1: Quick Reference
Jump straight to any section you need - the guide is designed for quick lookup during development.

### Option 2: Learn from Scratch
Start from the beginning and work through each section:

1. **Quick Start** - Download and run PocketBase
2. **Core Concepts** - Understand collections and security
3. **Client-Side Integration** - Connect your frontend
4. **Authentication** - Implement user management
5. **Advanced Topics** - Customize and extend

## 📖 How to Use This Guide

### 🔍 Quick Lookup
Each section is self-contained with practical examples. Use the table of contents to jump to what you need.

### 💡 Learning Path
Follow the sections in order for a complete understanding of PocketBase capabilities.

### 🛠️ Development Reference
Keep this open while coding - examples are copy-paste ready with minimal modification needed.

## 🌟 Key Features of This Reference

### ✨ Comprehensive Coverage
- **Client-side** JavaScript SDK with all methods and options
- **Server-side** JavaScript hooks and extensions
- **Admin operations** for managing collections and settings
- **Security patterns** and API rules
- **File handling** and realtime features

### 🎯 Practical Examples
Every concept includes working code examples that you can adapt for your use case.

### 📱 Real-world Patterns
Common application patterns like:
- User authentication and profiles
- Multi-tenant SaaS applications
- Content management systems
- File galleries and uploads
- Real-time chat applications

### 🔧 Production Ready
Deployment strategies, security best practices, and performance optimization tips.

## 🏗️ What You Can Build

With PocketBase and this guide, you can quickly build:

- **📱 Mobile Apps** - React Native, Flutter, native iOS/Android
- **🌐 Web Applications** - React, Vue, Svelte, vanilla JS SPAs  
- **💻 Desktop Apps** - Electron, Tauri, native applications
- **🤖 CLI Tools** - Command-line applications with data persistence
- **🔌 API Services** - Custom backends with authentication and realtime features

## 🎓 Learning Approach

This guide follows a **practical-first approach**:

1. **See the code** - Working examples for every concept
2. **Understand the why** - Explanations of when and why to use features  
3. **Apply the knowledge** - Patterns and best practices for real applications
4. **Troubleshoot issues** - Common problems and their solutions

## 🔗 Related Resources

- **Official PocketBase Docs**: [pocketbase.io/docs](https://pocketbase.io/docs/)
- **JavaScript SDK**: [GitHub Repository](https://github.com/pocketbase/js-sdk)
- **Dart SDK**: [GitHub Repository](https://github.com/pocketbase/dart-sdk)
- **Community Examples**: Check the PocketBase GitHub discussions

## 📝 Contributing

Found an error or want to add an example? This reference is designed to evolve with the PocketBase ecosystem. Contributions for:

- Additional code examples
- New use case patterns  
- Performance optimization tips
- Updated API references
- Troubleshooting solutions

## ⚖️ License

This reference guide is provided as-is for educational and development purposes. PocketBase itself is open source - check their repository for licensing details.

## 🚨 Version Note

This reference is based on **PocketBase v0.27+**. While most concepts remain stable, always check the official documentation for the latest API changes and features.

---

**Ready to build something awesome with PocketBase?** 🚀

Start with the Quick Start section and begin building your next application with one of the most developer-friendly backends available!
