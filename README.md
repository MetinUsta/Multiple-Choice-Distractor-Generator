<a name="readme-top"></a>


<br />
<div align="center">
  <h3 align="center"><b>Generating Wrong Answers Right: An NLP Pipeline for Distractor Creation</b></h3>

  <p align="center">
    An NLP pipeline for generating distractors in question-answering systems using context-based entity replacement and multiple choice question evaluation.
  </p>
</div>


## Table of Contents
<!-- TABLE OF CONTENTS -->
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://example.com)

The goal of our project was to develop a natural language processing pipeline that could generate distractors for question-answering systems. To accomplish this, we fine-tuned the distilbert-uncased model on the SQUAD dataset to enable it to generate answers. We then used a pre-trained NER model from the Spacy library to identify named entities in the generated answers.

To generate the distractors, we replaced the named entities with same-class entities from the context. For example, if the named entity in the generated answer was a person, we would look for other person entities in the context to use as distractors. To evaluate the effectiveness of our approach, we used a pre-trained model from HuggingFace named "T5-base fine-tuned on QASC" which is specifically designed for multiple choice question answering.

Our pipeline allows for the generation of distractors that are contextually relevant, which can help improve the overall performance of question-answering systems. Additionally, our approach allows for the creation of distractors that are different from the correct answer, but still plausible, which can be useful for training and evaluating question-answering systems.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With
[![HuggingFace][Huggingface.co]][Huggingface-Url] [![Spacy][Spacy.io]][Spacy-Url] [![Pytorch][Pytorch.org]][Pytorch-Url]


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started
### Prerequisites
Before running our NLP pipeline, it is necessary to have Jupyter Notebook installed on your machine, along with Python 3 and the following libraries:
  ```sh
  transformers
  datasets
  evaluate
  sentencepiece
  spacy
  ```

### Installation
To use our NLP pipeline, please follow the steps below:

1. Clone the repository to your local machine.

2. Install Python 3 (if not already installed) from the official website:
    https://www.python.org/downloads/
3. Install the required libraries by running the following command in your terminal or command prompt:

    ```sh
    pip install transformers datasets evaluate sentencepiece spacy
    ```

4. Launch Jupyter Notebook and open the three Jupyter notebooks included in the repository:
    * QuestionAnswering.ipynb
    * DistractorGenerator.ipynb
    * DistractorEvaluation.ipynb

5. Follow the instructions in the notebooks to run the pipeline.

Please note that the pipeline has been tested on Google Colab, and some of the file paths in the notebooks may point to Google Drive directories. You may need to modify these paths accordingly to ensure that the notebooks work correctly.
<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contributors

Metin Usta - metin.usta01@hotmail.com

Muhannad Tuameh - muhannadtumah@gmail.com

Project Link: [https://github.com/MetinUsta/Multiple-Choice-Distractor-Generator](https://github.com/MetinUsta/Multiple-Choice-Distractor-Generator)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Hugging Face](https://huggingface.co/)
* [Pretrained Multiple Choice Question Answering Model](https://huggingface.co/mrm8488/t5-base-finetuned-qasc)
* [Spacy](https://spacy.io/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: Assets/Block_Diagram.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com

[Huggingface.co]: https://img.shields.io/badge/-%F0%9F%A4%97Hugging%20Face-FFFFFF?logo=&style=for-the-badge

[Huggingface-Url]: https://huggingface.co/

[Spacy.io]: https://img.shields.io/badge/-Spacy-FFFFFF?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz4NCjwhLS0gR2VuZXJhdG9yOiBBZG9iZSBJbGx1c3RyYXRvciAxOC4wLjAsIFNWRyBFeHBvcnQgUGx1Zy1JbiAuIFNWRyBWZXJzaW9uOiA2LjAwIEJ1aWxkIDApICAtLT4NCjwhRE9DVFlQRSBzdmcgUFVCTElDICItLy9XM0MvL0RURCBTVkcgMS4xLy9FTiIgImh0dHA6Ly93d3cudzMub3JnL0dyYXBoaWNzL1NWRy8xLjEvRFREL3N2ZzExLmR0ZCI+DQo8c3ZnIHZlcnNpb249IjEuMSIgaWQ9IkViZW5lXzEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHg9IjBweCIgeT0iMHB4Ig0KCSB2aWV3Qm94PSIwIDMwOC41IDU5NS4zIDIxMyIgZW5hYmxlLWJhY2tncm91bmQ9Im5ldyAwIDMwOC41IDU5NS4zIDIxMyIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSI+DQo8cGF0aCBmaWxsPSIjMDlhM2Q1IiBkPSJNNzMuNywzOTUuMmMtMTMuNS0xLjYtMTQuNS0xOS43LTMxLjgtMTguMWMtOC40LDAtMTYuMiwzLjUtMTYuMiwxMS4yYzAsMTEuNiwxNy45LDEyLjcsMjguNywxNS42DQoJYzE4LjQsNS42LDM2LjIsOS40LDM2LjIsMjkuNGMwLDI1LjQtMTkuOSwzNC4yLTQ2LjIsMzQuMmMtMjIsMC00NC4zLTcuOC00NC4zLTI4YzAtNS42LDUuNC0xMCwxMC42LTEwYzYuNiwwLDguOSwyLjgsMTEuMiw3LjQNCgljNS4xLDksMTAuOCwxMy44LDI1LDEzLjhjOSwwLDE4LjItMy40LDE4LjItMTEuMmMwLTExLjEtMTEuMy0xMy41LTIzLTE2LjJjLTIwLjctNS44LTM4LjUtOC44LTQwLjYtMzEuOA0KCWMtMi4yLTM5LjIsNzkuNS00MC43LDg0LjItNi4zQzg1LjYsMzkxLjQsNzkuOCwzOTUuMiw3My43LDM5NS4yeiBNMTcwLjksMzYwLjhjMjguNywwLDQ1LDI0LDQ1LDUzLjZjMCwyOS43LTE1LjgsNTMuNi00NSw1My42DQoJYy0xNi4yLDAtMjYuMy02LjktMzMuNi0xNy41djM5LjJjMCwxMS44LTMuOCwxNy41LTEyLjQsMTcuNWMtMTAuNSwwLTEyLjQtNi43LTEyLjQtMTcuNXYtMTE0YzAtOS4zLDMuOS0xNSwxMi40LTE1DQoJYzgsMCwxMi40LDYuMywxMi40LDE1djMuMkMxNDUuNCwzNjguNywxNTQuNywzNjAuOCwxNzAuOSwzNjAuOHogTTE2NC4xLDQ0Ny42YzE2LjgsMCwyNC4zLTE1LjUsMjQuMy0zMy42DQoJYzAtMTcuNy03LjYtMzMuNi0yNC4zLTMzLjZjLTE3LjUsMC0yNS42LDE0LjQtMjUuNiwzMy42QzEzOC41LDQzMi43LDE0Ni43LDQ0Ny42LDE2NC4xLDQ0Ny42eiBNMjM1LjQsMzg4LjhjMC0yMC42LDIzLjctMjgsNDYuNy0yOA0KCWMzMi4zLDAsNDUuNiw5LjQsNDUuNiw0MC42djMwYzAsNy4xLDQuNCwyMS4zLDQuNCwyNS42YzAsNi41LTYsMTAuNi0xMi40LDEwLjZjLTcuMSwwLTEyLjQtOC40LTE2LjItMTQuNA0KCWMtMTAuNSw4LjQtMjEuNiwxNC40LTM4LjYsMTQuNGMtMTguOCwwLTMzLjYtMTEuMS0zMy42LTI5LjRjMC0xNi4yLDExLjYtMjUuNSwyNS42LTI4LjdjMCwwLjEsNDUtMTAuNiw0NS0xMC43DQoJYzAtMTMuOC00LjktMTkuOS0xOS40LTE5LjljLTEyLjgsMC0xOS4zLDMuNS0yNC4zLDExLjJjLTQsNS44LTMuNSw5LjMtMTEuMiw5LjNDMjQwLjgsMzk5LjMsMjM1LjQsMzk1LjEsMjM1LjQsMzg4Ljh6IE0yNzMuOCw0NTAuNw0KCWMxOS43LDAsMjgtMTAuNCwyOC0zMS4xdi00LjRjLTUuMywxLjgtMjYuNyw3LjEtMzIuNSw4Yy02LjIsMS4yLTEyLjQsNS44LTEyLjQsMTMuMUMyNTcuMSw0NDQuMywyNjUuMyw0NTAuNywyNzMuOCw0NTAuN3oNCgkgTTQxOC41LDMyMS43YzI3LjgsMCw1Ny45LDE2LjYsNTcuOSw0M2MwLDYuOC01LjEsMTIuNC0xMS44LDEyLjRjLTkuMSwwLTEwLjQtNC45LTE0LjQtMTEuOGMtNi43LTEyLjMtMTQuNi0yMC41LTMxLjgtMjAuNQ0KCWMtMjYuNi0wLjItMzguNSwyMi42LTM4LjUsNTFjMCwyOC42LDkuOSw0OS4yLDM3LjQsNDkuMmMxOC4zLDAsMjguNC0xMC42LDMzLjYtMjQuM2MyLjEtNi4zLDUuOS0xMi40LDEzLjgtMTIuNA0KCWM2LjIsMCwxMi40LDYuMywxMi40LDEzLjFjMCwyOC0yOC42LDQ3LjQtNTgsNDcuNGMtMzIuMiwwLTUwLjQtMTMuNi02MC40LTM2LjJjLTQuOS0xMC44LTgtMjItOC0zNy40DQoJQzM1MC41LDM1MS44LDM3NS44LDMyMS43LDQxOC41LDMyMS43TDQxOC41LDMyMS43eiBNNTc3LjUsMzYwLjhjNy4xLDAsMTEuMiw0LjYsMTEuMiwxMS44YzAsMi45LTIuMyw4LjctMy4yLDExLjhsLTM0LjIsODkuOQ0KCWMtNy42LDE5LjUtMTMuMywzMy0zOS4yLDMzYy0xMi4zLDAtMjMtMS4xLTIzLTExLjhjMC02LjIsNC43LTkuMywxMS4yLTkuM2MxLjIsMCwzLjIsMC42LDQuNCwwLjZjMS45LDAsMy4yLDAuNiw0LjQsMC42DQoJYzEzLDAsMTQuOC0xMy4zLDE5LjQtMjIuNWwtMzMtODEuN2MtMS45LTQuNC0zLjItNy40LTMuMi0xMGMwLTcuMiw1LjYtMTIuNCwxMy4xLTEyLjRjOC40LDAsMTEuNyw2LjYsMTMuOCwxMy44bDIxLjgsNjQuOA0KCWwyMS44LTU5LjlDNTY2LjEsMzcwLjIsNTY2LjQsMzYwLjgsNTc3LjUsMzYwLjh6Ii8+DQo8L3N2Zz4NCg==&style=for-the-badge

[Spacy-Url]: https://spacy.io/

[Pytorch.org]: https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white

[Pytorch-Url]: https://pytorch.org/