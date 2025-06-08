# Hadoop MapReduce Character Count 📊

This project demonstrates how to build and run a simple **Hadoop MapReduce** application inside a Dockerized Hadoop environment on macOS. It counts the number of characters in a given text file and stores the output in HDFS.

## 🧰 Tools & Technologies

- Java
- Apache Hadoop (Single Node on Docker)
- VS Code
- GitHub
- macOS
- HDFS

## 🚀 How It Works

1. **Write Java Code**  
   The `CharacterCount.java` class defines the Mapper, Reducer, and Driver logic for processing text and counting character frequencies.

2. **Compile & Package**  
   The code is compiled and packaged into a JAR file using Hadoop’s Java tools.

3. **Upload Input File**  
   The input text file is uploaded to the Hadoop Distributed File System (HDFS).

4. **Run MapReduce Job**  
   The JAR file is executed to process the input and output results to an HDFS directory.

5. **Result**  
   Output files are retrieved from HDFS, showcasing character frequencies.

## 🔧 Setup & Usage

1. **Run Hadoop in Docker**  
   A single-node Hadoop container is launched from the terminal.

2. **Upload input file to HDFS**  
   ```bash
   hdfs dfs -mkdir /input
   hdfs dfs -put input.txt /input
Run the JAR file

bash
Copy
Edit
hadoop jar charcount.jar CharacterCount /input /output
View Output

bash
Copy
Edit
hdfs dfs -cat /output/part-r-00000
📁 Project Structure
graphql
Copy
Edit
├── CharacterCount.java
├── charcount.jar
├── input.txt
├── output/            # Contains result files from HDFS
├── Dockerfile         # (Optional) for custom Hadoop container
└── README.md
✅ Output Sample
css
Copy
Edit
A   8
B   2
C   3
...
📤 How to Push to GitHub
bash
Copy
Edit
git init
git add .
git commit -m "Add Hadoop Character Count MapReduce project"
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
👩🏽‍💻 Author
Elizabeth Orji
MSc Computer Science – University of East London
GitHub: @LizzyOrji123

yaml
Copy
Edit

---








