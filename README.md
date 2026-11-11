# Mini Paper Template

A free LaTeX template for students writing a short physics review paper. The paper follows **MMRC: Motivation, Method, Results, and Conclusion** and includes examples of equations, figures, citations, and an author contribution statement.

Download the template from [XMUM-PHYS/Mini_paper_template](https://github.com/XMUM-PHYS/Mini_paper_template).

**Students are encouraged to use Overleaf**, an online LaTeX editor. You can write your paper and generate its PDF in your browser without installing LaTeX on your computer.

## 1. Create an Overleaf account

1. Visit [Overleaf registration](https://www.overleaf.com/register).
2. Enter your email address and choose a password, then select **Create account**. You may use your university email address. Alternatively, select **Continue with Google** if you prefer.
3. Follow any email verification instructions shown by Overleaf.
4. Sign in to reach your projects dashboard.

If you already have an account, simply [log in](https://www.overleaf.com/login).

## 2. Import the template into Overleaf

1. Open the [GitHub repository](https://github.com/XMUM-PHYS/Mini_paper_template).
2. Select the green **Code** button, then **Download ZIP**.
3. In your Overleaf dashboard, select **New Project → Upload Project**.
4. Select the ZIP file you downloaded. You do not need to unzip it first.
5. Wait for Overleaf to open the uploaded project, then click **Recompile** to generate the PDF.
6. Rename your project so you can recognise it, for example `Physics Review - Group 3`.

You do not need Git or a GitHub account for this download-and-upload method. See [Overleaf's project upload guide](https://docs.overleaf.com/managing-projects-and-files/uploading-a-project) for help.

## 3. Start writing

Open the main `.tex` file—the file containing `\documentclass{iopconfser}`. This is where you write your paper.

- Replace the title, author names, affiliation, and email address.
- Replace the short instructions in each section with your own writing.
- Keep the four main sections: **Motivation, Method, Results, and Conclusion**.
- Replace dummy equations, figures, and references with material relevant to your chosen measurement.
- Keep the author contribution statement only if it accurately describes your group's work.
- Click **Recompile** regularly to check the PDF.

Keep `iopconfser.cls` in the project: it controls the document's appearance. You do not need to edit it. Lines beginning with `%` are comments and do not appear in the PDF.

## 4. Add figures and references

**Figures:** Upload your image, for example `detector.png`. Replace the entire placeholder box command with:

```latex
\includegraphics[width=0.8\linewidth]{detector.png}
```

Keep the surrounding `figure` environment, caption, and label. Include a labelled apparatus diagram and a key result figure from the publication, with proper attribution.

**References:** Edit `references.bib`, replacing dummy entries with real publications. Each entry has a unique key, such as `paper`. Cite that key in your text:

```latex
The measurement is described in reference~\cite{paper}.
```

Keep these lines near the end of your main file:

```latex
\bibliographystyle{unsrt}
\bibliography{references}
```

Only cited entries normally appear in the reference list. See [Overleaf's BibTeX guide](https://www.overleaf.com/learn/latex/Bibliography_management_with_bibtex) for examples.

## 5. Check and download your paper

Before submitting, remove all instructional text and placeholders, check figure attribution and references, and confirm that you have addressed the assignment requirements. Recompile and use **Download PDF** to save your paper.

## Quick help

- **Wrong document compiles:** In project settings, select your paper's `.tex` file as the **Main document**.
- **Files are inside an extra folder:** If compilation fails, move the template files to the project's top level, keeping any image subfolders together.
- **Missing class file:** Check that `iopconfser.cls` was included in the upload.
- **Citation shows `[?]`:** Check that the citation key matches the entry in `references.bib`, then try **Recompile from scratch** in the Recompile menu.
- **Image not found:** Check the uploaded filename, including capital letters and the extension.

New to LaTeX? Start with [Overleaf's Learn LaTeX in 30 minutes](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes).
