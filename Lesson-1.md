| Difficulty level: Beginner |
| --- |

# Lesson 1: Variables

In Visual Studio Code (VSCode), open a new file and save it as `Lesson1.ps1`. Solve the goals below.

Goal 1: Use Get-Process to retrieve a list of running processes and store them into a variable named $ProcessList

Goal 2: Sort the contents of $ProcessList using Sort-Object by the "Id" property

Bonus: Retrieve only the first 10 results using Select-Object

### Answers
<details><summary>CLICK ME</summary>

#### Goal 1
```[Array]$ProcessList = Get-Process```

#### Goal 2
```[Array]$ProcessList | Sort-Object -Property Id```

#### Bonus
```
[Int]$Result = 10
[Array]$ProcessList | Sort-Object -Property Id | Select-Object -First $Result
```

</details>