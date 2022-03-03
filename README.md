# NUST BS/MS/PhD Thesis Style

The project is accessible as an [Overleaf template](https://www.overleaf.com/latex/templates/nust-seecs-thesis/bmkdkrfxqdmb)

For the moment I have added a few NUST schools, being an open-source project, I will be happy to get valuable [feedback and additional](https://github.com/hasanalikhattak/nust-thesis/issues) features from colleagues and students to further stabilize and improve the project, Happy exploring

Hasan Ali Khattak
https://github.com/hasanalikhattak

## Document Style and Packages

```TeX
\documentclass[12pt,a4paper,oneside]{book} %scrbook book report

\usepackage{graphicx}
\usepackage{astron}
\usepackage{nust}
```

## Title Page
```TeX
\title{Main Title}
\subtitle{Optional sub-title}

\author{Student Name}
\regno{Student Registration}
\degree{\MSIT} % MSCSE, MSCCS
\school{\SEECS}

\adviser{Supervisor}
\adviserAffiliation{Department of Computing}

\date{February 2022}

% \setcounter{tocdepth}{2}
% \setstretch{1.1}
% \linespread{1.1}

\begin{document}
\maketitle
```

## Pre-Content Pages

```TeX
\evaluationcommitteeapproval{Member 1}{Member 2}{Member 3}

\chapter*{Abstract}
Abstract\ldots

\certificateoforiginality

\chapter*{Acknowledgment}
This sample thesis is adopted from~\cite{Chinneck99}, a guide for organizing
thesis. See the reference for complete details.

\begin{center}
\emph{This work was supported by grants from XYZ, and also by the 
ABC project which is funded by PQR under the contract K-123456/789.}
\end{center}


\tableofcontents
\listoffigures
\listoftables
% \lstlistoflistings

\resetpagenumbering
```

## Definitions
```TeX
\begin{definition}[Testing 1,2,3]
This definition is placed within a chapter so is its number.
\end{definition}
```

## Figures
```TeX
\begin{figure}[htp]
\begin{center}
  \includegraphics[width=0.7\columnwidth]{nust.jpg}
  \caption{NUST Emblem.}
  \label{f-nust}
\end{center}
\end{figure}
```

## Table and Citations

```TeX
\begin{table}[h]
\centering
% Use, for example, p{3.5cm} style for fixed sized columns
% consider using vbox to ensure large text is wrapped inside a column
\begin{tabular}{|l|l|}
\hline
\textbf{Reference Type} & \textbf{Citation}\\ \hline
Article & \cite{khattak2019perception}\\ \hline
Book & \cite[p.127-133]{khattak2019perception}\\ \hline
InProceedings & \cite{khattak2019perception}\\ \hline
InCollection & \cite{khattak2019perception}\\ \hline
PhD Dissertation & \cite{khattak2019perception}\\ \hline
Masters Thesis & \cite{khattak2019perception}\\ \hline
Technical Report & \cite{khattak2019perception}\\ \hline
Misc & \cite{khattak2019perception}\\ \hline
\end{tabular}
\caption{Citation Styles.}
\label{t-References}
\end{table}
```

## Appendix Example
```TeX
\appendix
\chapter{First Appendix}
```
Separate numbering of appendices is also supported by LaTeX. The \textit{appendix} macro can be used to indicate that following chapters are to be numbered as appendices. Only use the \textit{appendix} macro once for all appendices.

## Bibliography Style

```TeX
\bibliographystyle{apa}
```


## Thesis Contents
### Introduction and Motivation

This is a general introduction to what the thesis proposal is all about. Keep in mind that it is not just a description of the contents of each section. Briefly summarize the research question(s), some of the reasons why it is a worthwhile question. Details of these questions will be stated in the later sections. It also recommended giving a birds-eye-view of the candidate solutions and possible out comes.


### Problem Statement and Contribution
Different disciplines have varying naming conventions. In engineering, thesis tend to refer to problem(s) to be solved where other disciplines talk in terms of question(s) to be answered. In either case, this section has three main parts:

* A concise statement of the question(s) that your thesis shall tackle.
* Justification, by direct reference to literature review from previous section that your question is previously unanswered.
*  Discussion of why it is worthwhile to answer this question.

Since this is one of the sections that the readers are definitely looking for, describe the issues more clearly by dividing this section into multiple subsections such as a spate section for **Aims**, another for listing **Original Contributions**, and yet another for mentioning the **Limitations**.


### Literature Review

Here you review the state of the art relevant to your thesis proposal. The idea is to present the major ideas in the state of the art right up to, but not including, your own personal brilliant ideas.

Critical analysis and comparisons should be made by pointing out the weakness of existing solutions and strengths of your proposal. You organize this section by idea, and not by author or by publication.

In certain situations, a background of the underlying concepts is required for better understanding of the research problem and also to improve the flow of the thesis. This could either be made an introductory part of this section or separately written in a prior section.


### Design and Methodology

This part of the thesis is much more free-form. It may have several subsections. But it all has only one purpose: to convince the examiners about the answer to the research question(s) or solution to the problem(s) that you set for yourself in the proposal.


### Implementation and Results

So show what you did so far (implementation and testing) that is relevant to answering the question(s) or solving the problem(s).


### Conclusion

You generally cover two things in this section, and each of these usually merits a separate subsection: **Conclusions** and **Summary of Contributions**.

Conclusions are not a rambling summary of the thesis: they are short, concise statements of the inferences made in this thesis. It helps to organize these as short numbered paragraphs, ordered from most to least important. All conclusions should be directly related to the research question(s) stated earlier.

The Summary of Contributions will be much sought and carefully read by the examiners. Here you list the contributions of new knowledge that your thesis would make. Of course, the thesis itself must substantiate any claims made here. There is often an overlap with the conclusions, but that's okay. Concise numbered paragraphs are again best. Organize from most to least important.
