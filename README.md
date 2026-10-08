1. What would happen if an ArrayList was used instead of a HashSet? Is there an advantage to using a HashSet here?

2. We chose: ```java HashMap<String, HashSet<Movie>>``` for the tracker, which made it very easy to answer questions such as "What movies has Alice watched" or "What is Alice's total viewing time". Explain how a different design, such as ```javaHashMap<Movie, HashSet<String>>``` would make certain other questions very easy to answer and others more difficult.

[Markdown Guide](https://www.markdownguide.org/basic-syntax/)
