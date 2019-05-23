| Difficulty level: Beginner |
| --- |

# Lesson 3: Storing Data

In Visual Studio Code (VSCode), open a new file and save it as `Lesson3.ps1`. Solve the goals below.

Goal 1: Create a new variable named $File and store the string "Lesson-3.json" to reference a JSON file saved in the root of this repository's folder.

Goal 2: Use Get-Content to retrieve the contents from the `$File` path. Hint: You will need to use the "-Raw" parameter to prevent the parser from formatting the data.

Goal 3: Use ConvertFrom-Json to convert the raw JSON data into a PowerShell native hashtable object. Store the results in `$ContentNative`.

Bonus: Display the contents of key6.

### Answers
<details><summary>CLICK ME</summary>

#### Goal 1
```
$File = 'lesson04.json'
```

#### Goal 2
```
$Content = Get-Content -Raw -Path $File
```

#### Goal 3
```
$ContentNative = ConvertFrom-Json -InputObject $Content
```

#### Bonus
```
Write-Output $ContentNative.key6
```

</details>