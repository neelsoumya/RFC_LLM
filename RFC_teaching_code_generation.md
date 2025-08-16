
Network Working Group                                     Soumya Banerjee
Request for Comments:                            
Category: Informational                                       August 2025
ISSN: 2070-1721


          Prompting Large Language Models for Simple Code
                  Generation in Biology Education

Status of This Memo

   This memo provides information for the Internet community.  It does
   not specify an Internet standard of any kind.  Distribution of this
   memo is unlimited.

Abstract

   This document proposes simple, standardized prompting techniques for
   using Large Language Models (LLMs) to generate computer code for
   biology education. The goal is to ensure that generated code is
   clear, easy to understand, and free from unnecessary technical
   complexity, making it suitable for biologists with limited
   programming experience.

Table of Contents

   1. Motivation
   2. Scope
   3. Prompting Guidelines
        3.1 General Principles
        3.2 Example Prompts
        3.3 Reinforcement Strategy
   4. Example Output
   5. Security and Ethical Considerations
   6. Conclusion
   7. References
   8. Acknowledgments

---

# 1. Motivation

Biologists often need to automate simple analyses (e.g., reading data,
plotting results, or calculating statistics). Modern LLMs (such as
ChatGPT, GPT-5, etc.) can assist by generating usable code. However,
without clear prompts, the output may be too technical or complicated.
This RFC establishes a consistent prompting style to promote
**simplicity, readability, and educational value**.

# 2. Scope

This RFC applies to the use of LLMs in **educational and teaching
settings** for biology students. It does not define best practices for
advanced software engineering or large-scale bioinformatics pipelines.

# 3. Prompting Guidelines

## 3.1 General Principles

- **Simplicity First**: Always request minimal, direct code with comments.  
- **Language Choice**: Prefer Python or R (widely used in biology).  
- **Clarity**: Ask the LLM to explain the code briefly after generation.  
- **Avoid Jargon**: Prompts should emphasize plain explanations.  

## 3.2 Example Prompts

**Example 1: Reading Data**  
```

Write simple Python code to read a CSV file called genes.csv and print
the first five rows. Please keep the code easy to understand, with
comments for a beginner biologist.

```

**Example 2: Plotting Data**  
```

Generate R code that plots a histogram of gene expression values stored
in a file expression.csv. Use simple functions and add comments so a
biology student can follow easily.

```

**Example 3: Basic Statistics**  
```

Give me Python code to calculate the mean and standard deviation of a
list of numbers representing cell counts. Keep the code very simple and
explain what each step does.

```

## 3.3 Reinforcement Strategy

When the LLM generates overly technical code, add this instruction to
the prompt:  

```

Please simplify the code further and remove any advanced or unnecessary
steps.

```

# 4. Example Output

**Prompt:**  
```

Write simple Python code to calculate the mean of a list of numbers.

````

**LLM Output:**

```python
# A simple example: calculating the mean of numbers
numbers = [2, 4, 6, 8, 10]

# Calculate mean by dividing the sum by the number of items
mean_value = sum(numbers) / len(numbers)

print("The mean is:", mean_value)
````

# 5. Security and Ethical Considerations

* Generated code must not be used blindly; students should **review and
  test** results.
* Instructors must clarify that LLMs may generate errors and that
  **understanding the logic** is more important than copying code.

# 6. Conclusion

This RFC outlines a lightweight framework for prompting LLMs to generate
**clear and beginner-friendly code** for biology education. By following
these guidelines, instructors can create a safe and effective learning
environment that emphasizes **understanding, not complexity**.

# 7. References

* Crocker, S. "RFC 1: Host Software," 1969.
* Internet Engineering Task Force (IETF). RFC Editor Series.
* Examples of practical RFCs: RFC 791 (IP), RFC 2616 (HTTP/1.1).

# 8. Acknowledgments

The author thanks biology students and educators who inspired the need
for simplified coding practices and effective prompting strategies.

```
