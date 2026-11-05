# Lab 4 WebSocket -- Project Report

## What I specified

Before choosing the message I would send in the test, I would bootup the server and in Postman, I would try different messages 
and see if sending the message multiple times, the output wouldn't chage.

The final message I've decided to use in the test is `your mother`, and the expected answer is `We were discussing you, not me.`


## What I changed

I've only changed `*/src/test/kotlin/websockets/ElizaServerTest.kt`


## Technical decisions

I've chose that message, because it always answers with the same message

## How I verified

To check that the tests ran correctly and passed, I've used `./gradlew check`.
At first, I've noticed the test was constantly sending messages. This was because I was checking for the `---` message
to send my text. I've changed it so it only send my message once the server sends `What's on your mind?`

## AI disclosure

Fill **either** the list **or** the no-AI line.

- **Tools / skills:** Claude Opus 5.5
- **Purpose:** To check how to send a message in the test
- **Representative prompts:** In this test, how do I send a message?
- **Affected files/sections:** `*/src/test/kotlin/websockets/ElizaServerTest.kt`
- **Validation steps:** ran `./gradlew check` to make sure it ran correctly
- **Human-reviewed:** I've made sure the answer it gave me was correct and wasn't non-sensical
