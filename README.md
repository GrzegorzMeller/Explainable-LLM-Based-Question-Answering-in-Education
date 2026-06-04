# Towards Explainable LLM-Based Question Answering in Education: Supporting Provenance Understanding and Trust Through Interactive Explanation Artifacts

<p>This repository serves as an online appendix accompanying the paper "Towards Explainable LLM-Based Question Answering in Education: Supporting Provenance Understanding and Trust Through Interactive Explanation Artifacts."</p>

<p>As the paper adopts a design-oriented perspective, many aspects of the proposed system are best understood through the user interface. Due to space constraints and limitations on figure size, it is not possible to include all interface components and screens in sufficient resolution within the paper itself. This repository therefore, provides additional materials that document the design of the system and support a more detailed understanding of the application that participants interacted with during the user study.</p>

<p>This README serves as the primary entry point and contains descriptions of the interface components, their intended purpose, and their role within the study. High-resolution screenshots of the system can be found in the <a href="screens/">Screens Folder</a>. To support transparency and reproducibility of the qualitative analysis, the repository also includes the complete thematic analysis <a href="Codebook.pdf">Codebook</a> used for coding participant transcripts, including code definitions and examples.</p>


<img width="100%" height="94.59%" alt="main" src="https://github.com/user-attachments/assets/4c6f104a-7b79-42bf-8dc1-e8b0c54fa838" />
<div height="20px"></div>
<p>Figure 1. User Interface of the second stimulus used during the user study. Key interface components (number next to the letter indicates that component opens on demand, after clicking on the parent component): the User Question (A), while the Chatbot’s Answer (C), the Graph Visualization (D), the  Textual Explanation of an Extracted Node (D.1), the Quiz Scaffold (D.2, D.4), the Forum Scaffold (D.3), the Extracted Learning Materials (E), the Faithfulness Score (B), the Faithfulness Table (B.1).</p>


<br />
<h2>3 stimuli presented during user studies</h2>
<p>Three screens are shown below, corresponding to the first, second, and last stimuli used in the user study. Screens in this repository are static images, but during the user study, participants could freely interact with them, particularly with graph nodes, learning materials, and uncertainty, which opened additional details on demand (as visualized in Figure 1: B.1, D.1 - D.4), . The order is from high confidence to high uncertainty. These scenarios mirror real cases coming from the Online Forum and Quiz Questions imposed in the previous academic year of the <i>anonymous</i> course. In these exemplars, uncertainty indicators qualitatively tracked the instructor-judged evaluation of responses, allowing us to examine whether participants noticed and made use of this signal.</p>

<br />
<p>Stimulus 1</p>
<img width="100%" height="63.08%" alt="condition1" src="https://github.com/user-attachments/assets/78917de1-b270-4d4b-80e6-538f49ec4bd8" />

<p>Stimulus 2</p>
<img width="5160" height="3255" alt="condition2" src="https://github.com/user-attachments/assets/d6c236d5-7cb0-4b86-bb35-c8ffcdb6d84e" />

<p>Stimulus 3</p>
<img width="5160" height="3255" alt="condition3" src="https://github.com/user-attachments/assets/73635bad-5d1d-476d-9bac-2492c7bc0c8a" />

<h2>Learning Analytics Integration</h2>
<img width="3201" height="2076" alt="learninganlytics" src="https://github.com/user-attachments/assets/22a8de40-9367-4413-8b23-3776282e8a60" />
<p> To complement explainability with pedagogical context, the knowledge graph was enriched with Learning Analytics (LA) scaffolds derived directly from the learning management system (EdX). Unlike traditional LA dashboards that present performance across an entire course, the scaffolds are contextualized to the learner's current question. When the chatbot retrieves concepts relevant to a query, the graph additionally exposes learning traces associated with those concepts, such as quiz and exercise results. In the example shown, the learner achieved full marks on assessment activities related to Chapter 1, while their performance on Chapter 2 was substantially lower. By linking learning traces directly to the concepts involved in answer generation, the system provides personalized context about the learner's prior engagement with the queried topics. We investigated whether exposing this information alongside explanation artifacts could encourage learners to reflect on their current level of understanding, identify knowledge gaps, and adapt subsequent study activities. Beyond supporting reflection, this integration extends the role of the knowledge graph from an explanation artifact to a personalized learning interface, providing an additional rationale for visualizing the graph to end users.</p>

<h2>The Faithfulness Table</h2>
<img width="754" height="1109" alt="faithfulness_table_expanded" src="https://github.com/user-attachments/assets/c85526f5-b377-4469-8343-53b9f1802fd2" />
<p>This view corresponds to the Faithfulness Table component previously introduced as B.1 in Figure 1. The table provides a scrollable, statement-level inspection of the generated answer, allowing learners to examine each extracted claim individually. For every statement, the system displays (1) a support decision indicating whether the claim is supported by the retrieved course materials and (2) a textual explanation justifying that decision. These support decisions are subsequently aggregated to compute the overall faithfulness score presented elsewhere in the interface. Beyond uncertainty communication, the table can be viewed as a form of answer debugging, enabling learners to inspect which parts of the generated response are grounded in course content and which may require additional verification.</p>


<h2>XAI–LLM approach for theoretical QA</h2>
<img width="5850" height="1950" alt="framework" src="https://github.com/user-attachments/assets/a34fdd37-c672-4468-bd8c-398ec554dfc0" />
<p>Description is provided in Section 3.2 of the paper.</p>


<h2>Early design used during the co-design session</h2>
<img width="1318" height="1229" alt="File Upload (3)" src="https://github.com/user-attachments/assets/b2e1721b-70f5-4ac9-8e89-074075113e01" />


<p>This interface was used during the co-design session with educators and served as an early exploration of how explainability features could be integrated into an educational QA system. Feedback from the co-design session (as described in Section 3.1) highlighted two important limitations. For instance, participants expressed concerns that a single numerical confidence score (e.g., 85%) might be difficult to interpret and could encourage over-reliance on the system. Second, while the interface explained generated answers, it lacked a clear pedagogical value and provided little support for learner reflection. These observations directly informed the final design, leading to the introduction of richer confidence explanations, statement-level faithfulness inspection, and Learning Analytics scaffolds embedded within the knowledge graph to contextualize answers using the learner's own educational data.</p>
