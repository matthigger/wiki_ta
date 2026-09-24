# Scanning quizzes/exams

After a quiz or exam, we scan the paper copies, upload them to Gradescope,
and keep the paper. Students sometimes say we lost their work, so each step
below makes sure any page on Gradescope can be traced back to its paper
copy. Please forgive my sepcificity below, it has been motivated by chasing missing submissions in past semesters.

## 1. Scan the paper copies

1. Use scissors to cut off the stapled corner of each exam, so the pages come apart.
2. Check that every page with a problem on it has the student's name (students may only label the first one, re-label it if need be here)
3. Scan each question in stacks of `n=10` (double sided), saving to a USB drive.  Notice that a student's first page/question is sent to a different PDF than their second page/question.
4. Rename each PDF to something short and write that name on its paper stack.  A simple code works, like using a number for the page/question index and letter for the stack: `2c.pdf` is the second question's third stack of `n=10` submissions.

## 2. Create the assignment on Gradescope

1. Go to **Assignments > Create Assignment** and choose the type:
    - **Exam / Quiz**: use this for quizzes and exams. Every student's answer to a question is in the same spot on the same page.
    - **Homework / Problem Set**: Students put their work wherever they like, not typical of exams.
    NOTE: for DS4400sp26 each question should get its own gradescope assignment.  So a quiz with two questions creates two distinct gradescope assignments.  (This will allow for our backend to easily swap in a student's maximum score, should they choose to re-take a question)
2. Upload the blank student copy of the quiz/exam as the template.
   Gradescope uses it to find each answer on every student's scan. It must
   have the same number of pages as one student's scan (if scans are double
   sided, count both sides).
3. Name the assignment exactly as the title on the quiz/exam, and set its
   date to the date printed on it. Leave the other grading settings at
   their defaults.
4. On the template, mark the box where students write their name, and the
   ID box (if there is one).
5. Build the outline, adding each question with the **New Question**
   button. Split questions into their smallest parts: graders would rather
   grade 6.i on its own than all of question 6 at once. For each question:
    - Use the question name printed on the quiz/exam.
    - Enter the points it's worth.
    - Draw a box on the template around where the answer goes. Keep the box
      as small as possible while still covering all of the student's work;
      Gradescope's AI-assisted grading groups similar answers, and it works
      best with tight boxes.
    - For extra credit questions, remove the point limit (ceiling).
6.  Click **Save Outline**.

## 3. Upload the scans to Gradescope

1. Head to **Manage Scans**.
2. Upload the PDFs from the USB drive, keeping their short names so each
   one matches its labeled paper stack.
3. Gradescope splits each PDF into one submission per student. Click
   **Show** on each PDF and check that it made exactly 10 submissions, each
   with the right number of pages.
    - If you see "Unable to confidently auto-split", scroll to the pages
      marked in yellow. Zoom in with the magnifying glass, then reorder,
      split, or merge pages until each submission is one complete exam.
      Then click **Create Submissions**.
    - Only delete a page if it is blank or scanned twice.
    - Warning: sometimes the scanner will pull two pages at once, effectively discarding a page.  This is why we scan in batches of 10, so that we can expect/validate that all 10 made it.
4. Gradescope tries to match each submission to a student using the name
   and ID boxes. Go to **Manage Submissions** and:
    - Open the **Unassigned** tab. For each submission there, type the
      student's name or ID and press Tab to assign it.
5. Before you finish, confirm that every submission is assigned to a
   student, and that the number of submissions equals the number of paper
   exams. If a count is off, the labelling and counting in stacks of 10 should help you find and scan any missing exams.
