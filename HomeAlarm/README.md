# 🏠 Home Alarm System

A fully-working & customizable home alarm app / low-cost system for our house.

## 📜 The Past Situation

The last system was rigid and hard-to-understand.

Being little more than a basic PHP website, the user had no clear image of what was going on in the alarm system, and making changes was a more difficult process that required knowledge of how it was internally structured and guesswork of what the very basic UI did.

## 💡 The Solution

This project solves the above problems, as it provides a **simple-to-use app** that visualizes the alarm system, the trap positions and what's armed and what's not. This makes arming & disarming more trivial and provides quick information about the current state of the alarm.

Crucially, it also covers an important security feature previously missed: **it notifies the user with an alarm when something goes wrong.**

Is an armed door open? The user is immediately notified on their phone with a loud alarm describing the situation.

## ⚙️ How Does It Work?

1. A user logs in normally and opens the app.
2. Information on open and armed doors is saved (& updated from Arduinos) in the backend server.
3. The server then sends the required data to the app to display.
4. Changes made in the app are instantly also reflected on the server.
5. When the server notices a change that shouldn't be (e.g. an armed door opened), it sends a **Firebase message** that triggers a full-screen notification on the user's phone to notify them of the situation.

## 🚀 Expansion Plans

- [ ] Giving different users different permissions so they can only change & view the alarm status on different floors of the apartment building.
- [ ] Better floor plan images for each floor to further improve visualization. (...ignore the current MS Paint-created image until I find real floor planning software...)

---

*More updates to come as the project evolves.*