# **AI Code Loop: একজন Software Engineer-এর জন্য AI ব্যবহারের সঠিক পদ্ধতি**

## **১. মূল ধারণা: AI কি Software Engineer-কে Replace করবে?**

**AI কোড লেখার কাজ সহজ করছে, কিন্তু Engineering-এর দায়িত্ব দূর করছে না।**

AI দিয়ে খুব সহজেই একটি সম্পূর্ণ Application, Dashboard, API কিংবা UI তৈরি করা সম্ভব। কিন্তু সুন্দর UI বা কাজ করা একটি Application মানেই সেটি Production-ready Software নয়।

একজন Software Engineer-এর দায়িত্ব শুধু কোড লেখা নয়। বরং:

- সঠিক Architecture নির্বাচন করা।
- Business Logic ঠিক রাখা।
- Security নিশ্চিত করা।
- Edge Cases বিবেচনা করা।
- Performance নিশ্চিত করা।
- Code Quality ও Maintainability বজায় রাখা।
- AI-এর তৈরি কোড সঠিক কিনা যাচাই করা।

### **Typing বনাম Thinking**

| বিষয়                    | AI-এর যুগে অবস্থা                    |
| ----------------------- | ------------------------------------ |
| Code Typing             | অনেক সস্তা ও সহজ হয়েছে               |
| Boilerplate Development | AI দ্রুত করে দিতে পারে               |
| Problem Solving         | এখনো Engineering Skill প্রয়োজন       |
| System Design           | Engineer-এর গুরুত্বপূর্ণ দায়িত্ব     |
| Security & Validation   | Engineer-কে নিশ্চিত করতে হবে         |
| Code Review             | অত্যন্ত গুরুত্বপূর্ণ                 |
| Testing                 | AI সাহায্য করবে, Engineer যাচাই করবে |

মূল কথা: **Typing is cheap. Engineering Thinking is expensive.**

## **২. AI-কে Junior Developer হিসেবে বিবেচনা করুন**

AI-কে নিজের পরিবর্তে একজন সম্পূর্ণ Software Engineer হিসেবে বিবেচনা না করে একজন Junior Developer বা Coding Assistant হিসেবে বিবেচনা করতে হবে।

Your Role

**Senior Software Engineer / Architect**

Requirements, Architecture, Business Logic, Decisions, Review

Task delegation & guidance

AI's Role

**Junior Developer / Coding Assistant**

Implementation, Boilerplate, Functions, Tests, Refactoring

Code review & validation

**Production-ready Software**

Engineer-approved implementation

আপনি AI-কে কাজ দেবেন, কিন্তু কী তৈরি হবে, কেন তৈরি হবে এবং কীভাবে সঠিকতা যাচাই হবে—সেই নিয়ন্ত্রণ আপনার হাতে থাকবে।

## **৩. AI Code Loop কী?**

AI Code Loop হলো AI-এর সাহায্যে Software Development করার একটি Engineering Workflow।

এখানে একটি বড় সমস্যাকে ছোট ছোট অংশে ভাগ করে, প্রতিটি অংশের জন্য নির্দিষ্ট নির্দেশনা দেওয়া হয় এবং প্রতিটি কাজ Test ও Verify করে পরবর্তী ধাপে যাওয়া হয়।

## **The 7-Step AI Code Loop**

1. **Write the Goal in One Sentence**

   একটি Feature-এর মূল উদ্দেশ্য এক বাক্যে লিখুন।
2. **Write the Rules — What Must Be True**

   কোন কোন Business Rules অবশ্যই মানতে হবে তা নির্ধারণ করুন।
3. **Write Two Examples**

   Input এবং Expected Output-এর উদাহরণ দিন।
4. **Write Two Bad Situations**

   Edge Cases ও Worst-case Scenarios উল্লেখ করুন।
5. **Ask AI for Small Pieces, Not the Whole Thing**

   পুরো Application না দিয়ে ছোট Function, Class বা Module তৈরি করতে বলুন।
6. **Ask for Tests and Run Them**

   AI-কে Test Case লিখতে এবং Test Run করতে বলুন। নিজেও ফলাফল যাচাই করুন।
7. **If Something Fails, Improve the Prompt and Repeat**

   ভুল হলে শুধু কোড পরিবর্তন নয়, প্রয়োজনে Requirement ও Prompt উন্নত করে Loop পুনরাবৃত্তি করুন।

এটাই AI Code Loop-এর মূল Framework।

## **৪. AI-কে Prompt দেওয়ার আগে Requirement Analysis করুন**

ভিডিওর একটি গুরুত্বপূর্ণ পরামর্শ হলো: সরাসরি ChatGPT, Claude বা Cursor খুলে Prompt লেখা শুরু করবেন না।

প্রথমে নিজের Requirement Note তৈরি করুন।

উদাহরণ হিসেবে একটি E-commerce Shopping Cart Module তৈরি করতে হলে:

**Requirement Note:**

1. Server-side Shopping Cart Total Calculation করতে হবে।
2. User শুধু Product ID এবং Quantity পাঠাতে পারবে।
3. User-এর পাঠানো Price কখনো Trust করা যাবে না।
4. নিজের Product Catalog ব্যবহার করতে হবে।
5. Unknown Product Handle করতে হবে।
6. Invalid Quantity Reject করতে হবে।
7. Subtotal, Discount, Tax এবং Final Total Calculate করতে হবে।
8. Money সঠিকভাবে দুই Decimal পর্যন্ত Round করতে হবে।
9. Test Case থাকতে হবে।

এই Requirement Note তৈরি করার পর AI-কে Prompt দিতে হবে।

এতে AI-কে কম অনুমান করতে হবে এবং আপনার Requirement অনুযায়ী কাজ করার সম্ভাবনা বাড়বে।

## **৫. বাস্তব উদাহরণ: E-commerce Shopping Cart**

ধরা যাক, AI-কে বলা হলো:

> Build me a complete E-commerce Shopping Cart Module.

AI হয়তো সুন্দর UI, Product List, Quantity Controls, Subtotal, Discount এবং Tax Calculation তৈরি করে দেবে।

কিন্তু এখানে একটি বড় Security Problem থাকতে পারে।

**সমস্যা: Client-side Price Manipulation**

ধরা যাক:

- Product Price: $100
- User Browser থেকে Request Modify করল।
- Submitted Price পরিবর্তন করে $1 করে দিল।
- Server যদি User-এর পাঠানো Price গ্রহণ করে, তাহলে Product মাত্র $1-এ কেনা সম্ভব।

**ভুল Implementation**

**Client / Browser**

Product ID + Quantity + Price + Total

**Server trusts client price**

Security Risk

**সঠিক Implementation**

**Client / Browser**

শুধু Product ID + Quantity

**Server retrieves trusted Product Price**

**Server calculates Subtotal, Discount, Tax & Total**

Safer Architecture

এই উদাহরণ থেকে শিক্ষা:

AI সুন্দর কোড তৈরি করতে পারে, কিন্তু Engineer-কে নিশ্চিত করতে হবে সেই কোড বাস্তব জীবনে নিরাপদ এবং সঠিকভাবে কাজ করছে কি না।

## **৬. Engineering-grade Prompt তৈরি করার নিয়ম**

একটি ভালো Prompt-এ নিচের বিষয়গুলো থাকা উচিত:

| Section      | কী দিতে হবে                       |
| ------------ | --------------------------------- |
| Context      | কী তৈরি করতে যাচ্ছেন              |
| Goal         | মূল উদ্দেশ্য                      |
| Rules        | বাধ্যতামূলক Business Rules        |
| Examples     | Input ও Expected Output           |
| Edge Cases   | অস্বাভাবিক পরিস্থিতি              |
| Scope        | AI-কে ঠিক কতটুকু কাজ করতে হবে     |
| Deliverables | কী কী Output দিতে হবে             |
| Testing      | কীভাবে Test করতে হবে              |
| Verification | কোড দেওয়ার আগে সম্ভাব্য ভুল যাচাই |

### **Reusable AI Code Loop Prompt Template**

নিচের Template-টি Cursor, Claude Code, ChatGPT, VS Code কিংবা অন্যান্য AI Coding Agent-এ ব্যবহার করতে পারবেন।

# AI Code Loop — Engineering Grade Prompt Template

## 1. Context

You are working as my Junior Software Engineer. I am responsible for the overall architecture, business logic, and final code review.

Your responsibility is to implement the specific task I assign, following my requirements strictly.

## 2. Goal

[Describe the main objective in one clear sentence.]

## 3. Rules — What Must Be True

Follow these rules strictly:

1. [Business Rule 1]
2. [Business Rule 2]
3. [Business Rule 3]
4. [Validation Rule]
5. [Security Rule]
6. [Expected behavior]

Do not invent additional business rules or make assumptions without asking.

## 4. Input & Output Examples

Example 1:\
Input: [Provide input]\
Expected Output: [Provide expected output]

Example 2:\
Input: [Provide input]\
Expected Output: [Provide expected output]

## 5. Edge Cases & Bad Situations

Handle the following scenarios:

1. [Invalid input]
2. [Missing or null values]
3. [Unexpected data]
4. [Boundary conditions]
5. [Other failure scenarios]

## 6. Implementation Scope

- Implement only the requested function, class, or module.
- Do not build the entire application.
- Follow the existing project architecture and coding conventions.
- Use the specified programming language and technologies.
- Avoid unnecessary dependencies.
- Do not modify unrelated files.
- Keep the implementation readable and maintainable.

## 7. Testing Requirements

- Write relevant unit tests.
- Cover normal scenarios and edge cases.
- Include negative test cases.
- Run the tests.
- Report actual test results.
- Do not claim tests passed unless they were executed successfully.

## 8. Deliverables

Provide:

1. Implementation code.
2. Test cases.
3. Test execution results.
4. Example output.
5. Any assumptions or limitations.

## 9. Mandatory Pre-Implementation Review

IMPORTANT: Before writing any code:

1. Analyze all requirements and rules.
2. List possible implementation mistakes.
3. Identify security risks and edge cases.
4. Verify whether the rules are clear and consistent.
5. Identify missing information or conflicting requirements.
6. Ask me for clarification if something is ambiguous.
7. Present your implementation plan and wait for my approval.

Do not start implementation until I approve the plan.

## 10. Final Verification

After implementation:

- Review the code against every requirement.
- Verify all business rules.
- Run the tests and report failures.
- Identify remaining risks.
- Confirm whether the implementation is ready for integration.

Remember: Correctness, security, maintainability, and testability are more important than simply generating code quickly.

**বিশেষ নির্দেশনা:** প্রতিটি Feature-এর জন্য Template ব্যবহার করবেন। একই Prompt দিয়ে পুরো Application তৈরি করতে যাবেন না।

## **৭. Beginner, Mid-level ও Senior Engineer-এর দায়িত্ব**

একই AI Code Loop সবাই ব্যবহার করতে পারবেন। তবে Experience অনুযায়ী দায়িত্বের গভীরতা আলাদা হবে।

| Level     | প্রধান দায়িত্ব                                                                       |
| --------- | ------------------------------------------------------------------------------------ |
| Beginner  | ছোট Function, Basic Rules, Input Validation ও Unit Tests                             |
| Mid-level | Complex Business Logic, Edge Cases, Error Handling, Integration                      |
| Senior    | Architecture, Security, Performance, Scalability, Maintainability ও Long-term Impact |

Senior Engineer-কে আরও কিছু বিষয় বিবেচনা করতে হবে:

- **Security:** কোথায় Vulnerability তৈরি হতে পারে?
- **Performance:** বড় Data হলে কত দ্রুত কাজ করবে?
- **Maintainability:** ৫–৬ বছর পরেও কোড Maintain করা সম্ভব হবে কি?
- **Scalability:** User ও Traffic বাড়লে System ঠিক থাকবে কি?
- **Integration:** ছোট Module-টি পুরো Application-এর সঙ্গে কীভাবে কাজ করবে?

## **৮. Software Engineer-এর জন্য Practical Workflow**

বাস্তব Project-এ নিচের Workflow অনুসরণ করতে পারেন।

## **AI-Assisted Development Workflow**

1. **Requirement Analysis**

   নিজে Requirement বুঝুন এবং Documentation তৈরি করুন।
2. **Architecture & Planning**

   Feature Breakdown, Database Structure, API Design নির্ধারণ করুন।
3. **AI Prompting**

   AI Code Loop Template ব্যবহার করে ছোট Task দিন।
4. **AI Implementation**

   AI-কে নির্দিষ্ট Function বা Module তৈরি করতে দিন।
5. **Code Review**

   Generated Code নিজে Review করুন।
6. **Testing & Validation**

   Unit Test, Integration Test এবং Manual Test করুন।
7. **Security & Performance Review**

   Vulnerability, Performance ও Edge Cases যাচাই করুন।
8. **Integration & Deployment**

   সবকিছু ঠিক থাকলে Main Application-এ Integrate করুন।

## **৯. যে ভুলগুলো কখনো করা উচিত নয়**

1. শুধু একটি Prompt দিয়ে সম্পূর্ণ Application তৈরি করতে দেওয়া।
2. AI-এর Generated Code Review না করে Accept করা।
3. Business Logic AI-এর অনুমানের ওপর ছেড়ে দেওয়া।
4. শুধু UI দেখে Application-কে Complete মনে করা।
5. Security ও Validation উপেক্ষা করা।
6. AI-এর লেখা Test Case-কে শতভাগ সঠিক ধরে নেওয়া।
7. Test Run না করেই Code Production-এ Deploy করা।
8. Project Architecture না বুঝে AI-কে সরাসরি Existing Codebase পরিবর্তন করতে দেওয়া।

## **১০. Final Engineering Principles**

ভিডিওটির মূল বক্তব্য থেকে সবচেয়ে গুরুত্বপূর্ণ শিক্ষাগুলো:

- AI ব্যবহার করতে হবে, কিন্তু অন্ধভাবে Trust করা যাবে না।
- Coding Fundamentals এখনো অত্যন্ত গুরুত্বপূর্ণ।
- Programming Logic না বুঝলে ভালো Engineering Prompt তৈরি করা কঠিন।
- বড় Problem-কে ছোট ছোট Independent Task-এ ভাগ করতে হবে।
- প্রতিটি Task-এর জন্য Rules, Examples ও Edge Cases দিতে হবে।
- AI দিয়ে Test লিখিয়ে নিতে হবে, কিন্তু Test Review নিজেকেও করতে হবে।
- Code Generation নয়, Correctness নিশ্চিত করাই Engineering-এর আসল দায়িত্ব।
- AI-কে Assistant হিসেবে ব্যবহার করতে হবে, Decision Maker হিসেবে নয়।

## **১১. নিজের শেখার জন্য Action Checklist**

**AI Code Loop Practice**

0/11 Completed

একটি Feature-এর Requirement Note তৈরি করা

Feature-টিকে ছোট ছোট Task-এ ভাগ করা

প্রতিটি Task-এর Goal নির্ধারণ করা

Business Rules ও Validation লিখে দেওয়া

কমপক্ষে দুটি Input/Output Example তৈরি করা

Edge Cases ও Worst-case Scenarios নির্ধারণ করা

AI দিয়ে Implementation তৈরি করা

AI দিয়ে Unit Tests তৈরি ও Run করা

নিজে Code Review করা

Security ও Performance যাচাই করা

সব Test Pass হলে Integration করা

Reset Checklist

## **আমার চূড়ান্ত মতামত**

একজন Full-stack বা Senior Software Engineer হিসেবে AI ব্যবহার করার সময় আপনার সবচেয়ে বড় শক্তি হওয়া উচিত তিনটি বিষয়:

**Thinking**

Problem Solving

**Engineering**

Architecture & Logic

**Verification**

Testing & Quality

**মনে রাখবেন:**

> A good developer writes code. A great engineer understands the problem, designs the solution, validates the implementation, and takes responsibility for the result.

AI আপনার Code লেখার গতি বাড়াতে পারে। কিন্তু আপনার Engineering Judgment, Technical Knowledge এবং Decision-making Skill-এর বিকল্প হতে পারে না।

এই Framework-টি নিজের পরবর্তী SmythOS বা Biteo Development Task-এ প্রয়োগ করে দেখতে পারেন। একটি ছোট Feature দিয়ে শুরু করাই সবচেয়ে ভালো।
