# QUIZ!! - JavaApplication45 - General Knowledge Quiz JAR

A Java Swing desktop quiz application built in NetBeans (JavaApplication45). The application displays a `QUIZ!!` window with 4 colored panels and validates answers instantly with GREEN Correct Answer! and RED Incorrect Answer! feedback.

### Project Title and Short Description
**JavaApplication45 - Calculation / Marks Quiz System**
A JFrame Form that asks 4 general questions. User enters text in JTextField and clicks Check. The system uses `.trim()` and `equalsIgnoreCase` for string checks and `Double.parseDouble` for numeric check. Same validation concept as my Portfolio contact form.

Questions:
1. Capital of France
2. Color of the sky
3. First name of the President of USA
4. Number of SA languages

### Live Website Link
Not applicable - This is a Java desktop JAR application, not a website.
**Executable JAR Location:** `dist/JavaApplication45.jar` after Clean and Build
**GitHub Repository:** https://github.com/tumieyndlovuu/JavaApplication45
**Portfolio that showcases it:** https://tumieyndlovuu.github.io/portfolio/

### Technologies Used
- **HTML, CSS, JavaScript:** Not used in this JAR - Java Swing used instead (for your Portfolio README you list these)
- **Java SE (Swing):** JFrame, JPanel, JLabel (lbl1, lbl2, lbl3, lbl4), JTextField (txt1, txt2, txt3, txt4), JButton (Check, jButton1, jButton2, jButton3)
- **IDE:** NetBeans  - tabs `calculation.java x`, Design / History view, Run Debug Profile menu
- **Layout:** GroupLayout - Header Blue "QUIZ!!" + 2x2 Grid: Teal panel, Dark Grey panel, Purple panel, Dark Blue panel
- **Logic:** `java.awt.event.ActionEvent` + `java.awt.Color`

### Features Included

1.  **4-Panel Quiz UI:** blue header QUIZ!!, 4 questions with input fields and Check buttons
2.  **Presence + Type + Format Validation:**
    - `String AnsOne=txt1.getText().trim();` - removes spaces
    - `if(AnsOne.equalsIgnoreCase("Paris"))` - case-insensitive check
3.  **Color Feedback (RED/GREEN):**
    - `lbl1.setText("Correct Answer!"); lbl1.setForeground(Color.green);`
    - `lbl1.setText("Incorrect Answer!"); lbl1.setForeground(Color.red);`
4.  **Numeric Validation for SA Languages:**
    ```java
    String AnsFour=txt4.getText().trim();
    double A1 = Double.parseDouble(AnsFour);
    if(A1==12){
      lbl4.setText("Correct Answer!");
      lbl4.setForeground(Color.green);
    }
