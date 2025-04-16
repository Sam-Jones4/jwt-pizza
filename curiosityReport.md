# 💡 Curiosity report

> "Curiosity is a defining characteristic of a successful software engineer."
> - Professor Jensen

## SQL Injection

While performing penetration testing in delverable 12, I really wanted to do a SQL injection attack. Unfortunately, I failed, and it was very difficult to find resources on how to perform these types of attacks. This is because it's illegal and classified as a cybercrime. That being said, I researched it a lot.

### What is it?

A SQL injection attack is essentially inputting lines of SQL commands where a website would require input. If done correctly, the code is accepted into the database and can do anything from alter data to destroy the entire database. It has the potential to be totally destructive and is classified as the OWASP number three largest security concern for web applications.

This is possible in two ways:
1. SQL injection into a String/Char parameter
2. SQL injection into a Numeric parameter

### Conclusion

Ultimately a lot of websites provide examples for types of SQL commands that are possible to inject. I learned about the types of injection and potential effects, but no website would provide actual curl command examples to perform the attack. Even generative AI like ChatGPT and Microsoft Copilot wouldn't provide information on how to perform the attacks– just ways to defend against it. This is because if anyone provided the info on how it is done, they could be liable for indirectly taking part in cybercrime. It's definitely for the best, and made for a good rabbit hole.
