# Scanning quizzes/exams

After a quiz or exam, we scan the paper copies, upload them to Gradescope, and keep the paper.
Students sometimes say we lost their work, so each step below makes sure any page on Gradescope can be traced back to its paper copy.
Please forgive how specific these steps are; each one comes from chasing missing submissions in past semesters.

## 1. Scan the paper copies

1. Cut off the stapled corner of each exam with scissors so the pages come apart.
2. Check that every page with a problem on it has the student's name.
   Students often write it only on the first page, so add it wherever it's missing.
3. Scan each question separately, in stacks of 10 (double sided), saving to a USB drive.
   A student's first question ends up in a different PDF than their second question.
4. Give each PDF a short name and write that name on its paper stack.
   A simple code works: a number for the question and a letter for the stack.
   For example, `2c.pdf` is the third stack of 10 for question 2.
5. Return the paper copies, still in their labeled stacks, to the instructor, who will keep them for the rest of the semester.

## 2. Create the assignment on Gradescope

1. Go to **Assignments > Create Assignment** and choose the type:
    - **Exam / Quiz**: use this for quizzes and exams.
      Every student's answer to a question is in the same spot on the same page.
    - **Homework / Problem Set**: students put their work wherever they like.
      This isn't typical for exams.

    !!! note "DS4400"
        Each question gets its own Gradescope assignment, so a quiz with two questions becomes two Gradescope assignments.
        This lets our backend easily swap in a student's best score if they retake a question.

2. Upload the blank student copy of the quiz/exam (or of just that question, if each question is its own assignment) as the template.
   Gradescope uses it to find each answer on every student's scan.
   It must have the same number of pages as one student's scan (if scans are double sided, count both sides).
3. Name the assignment exactly as the title on the quiz/exam, and set its date to the date printed on it.
   Leave the other grading settings at their defaults.
4. On the template, mark the box where students write their name, and the ID box (if there is one).
5. Build the outline, adding each question with the **New Question** button.
   Split questions into their smallest parts: graders would rather grade 6.i on its own than all of question 6 at once.
   For each question:
    - Use the question name printed on the quiz/exam.
    - Enter the points it's worth.
    - Draw a box on the template around where the answer goes.
      Keep the box as small as possible while still covering all of the student's work; Gradescope's AI-assisted grading groups similar answers, and it works best with tight boxes.
    - For extra credit questions, remove the point limit (ceiling).
6. Click **Save Outline**.

## 3. Upload the scans to Gradescope

1. Head to **Manage Scans**.
2. Upload the PDFs from the USB drive, keeping their short names so each one matches its labeled paper stack.
3. Gradescope splits each PDF into one submission per student.
   Click **Show** on each PDF and check that it made exactly 10 submissions, each with the right number of pages.
    - If you see "Unable to confidently auto-split", scroll to the pages marked in yellow.
      Zoom in with the magnifying glass, then reorder, split, or merge pages until each submission is one complete exam.
      Then click **Create Submissions**.
    - Only delete a page if it is blank or scanned twice.
    - Watch for pages the scanner pulled through two at a time, which skips a page.
      Scanning in batches of 10 means you know every PDF should hold exactly 10 submissions, so a missing page shows up.
4. Gradescope tries to match each submission to a student using the name and ID boxes.
   Go to **Manage Submissions**, open the **Unassigned** tab, and for each submission there, type the student's name or ID and press Tab to assign it.
5. Before you finish, confirm that every submission is assigned to a student, and that the number of submissions equals the number of paper exams.
   If a count is off, the stack labels and the counts of 10 will help you find and scan the missing exams.
