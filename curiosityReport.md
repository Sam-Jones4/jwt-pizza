# 💡 Curiosity report

> "Curiosity is a defining characteristic of a successful software engineer."
> – Professor Jensen

## SQL Injection

While performing penetration testing in delverable 12, I really wanted to do a SQL injection attack. Unfortunately, I failed, and it was very difficult to find resources on how to perform these types of attacks. This is because it's illegal and classified as a cybercrime. That being said, I researched it a lot.

### What is it?

A SQL injection attack is essentially inputting lines of SQL commands where a website would require input. If done correctly, the code is accepted into the database and can do anything from alter data to destroy the entire database. It has the potential to be totally destructive and is classified as the OWASP number three largest security concern for web applications.

This is possible in two ways:
1. SQL injection into a String/Char parameter
2. SQL injection into a Numeric parameter

Here are examples I got from OWASP on both:
```sh
SELECT * from table where example = 'Example'
```
```sh
SELECT * from table where id = 123
```

I learned that oftentimes the attacker will provide something that is always true in the input. For example they will say:
```sh
... OR '1'='1';
```
Since this is always true, they're essentially selecting anything from a certain table in the database. It's a safety net for if what they're searching for doesn't exist.
Another part of it is ending their input with "--" which comments out the rest of the code following their injection. I'm assuming this is to erase potential safety precautions that could've been written later in the code. Smart stuff!


### Conclusion

Ultimately a lot of websites provide examples for types of SQL commands that are possible to inject. I spent hours learning about the types of injections and potential effects, but no website would provide curl command examples to perform the attack. This is why my attempt at self attacking failed. Even generative AI like ChatGPT and Microsoft Copilot wouldn't provide information on how to perform the attacks– just ways to defend against it. This is because if anyone provided the info on how it is done, they could be liable for indirectly taking part in cybercrime. It's definitely for the best, and made for a good rabbit hole.
