🎨 ASCII Art Banner Generator
A powerful and customizable Go CLI tool that lets you generate ASCII art representations of strings in different styles and save them to a file.

✨ Features
🔤 Generate ASCII art from user-provided strings

💾 Save generated banners to .txt files

🖋 Supports multiple banner styles: standard, shadow, and more

🧰 Simple and flexible command-line usage

🛠 Easily extendable with new banner styles

🧰 Requirements
Go 1.18+

Go Modules enabled

🚀 Installation
git clone <repository_url>
cd <project_directory>
go mod tidy

⚙️ Usage
bash
Copy
Edit
go run . --output=<fileName.txt> "<STRING>" <BANNER_STYLE>

🧾 Arguments:
--output=<fileName.txt> → Output file (must end in .txt)

<STRING> → The text to convert into ASCII art

<BANNER_STYLE> → (Optional) Banner style:

standard

shadow

(More styles may be added in the future)

📦 Examples
Example 1 – Standard Banner
bash
Copy
Edit
go run . --output=banner.txt "hello" standard
banner.txt output:

 _              _   _          
| |            | | | |         
| |__     ___  | | | |   ___   
|  _ \   / _ \ | | | |  / _ \  
| | | | |  __/ | | | | | (_) | 
|_| |_|  \___| |_| |_|  \___/  
                              
🧑‍💻 Development
Want to add your own custom style?

Each banner style is defined as a separate function.

Simply add a new function that accepts a string and returns ASCII art.

🧪 Testing
Add unit tests to ensure your banner styles and file handling logic work correctly.

To run tests (if implemented):

bash
Copy
Edit
go test ./test