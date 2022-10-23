<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

# Table of content

- [Table of content](#table-of-content)
  - [About The Project](#about-the-project)
    - [Built With](#built-with)
  - [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
  - [Usage](#usage)
  - [Contributing](#contributing)
  - [Contact](#contact)
  - [Acknowledgments](#acknowledgments)


<br></br>
<!-- ABOUT THE PROJECT -->
## About The Project

**The objective** is to create an algorithm that retrieves the logos of the companies present on the documents. In this way, we will identify the companies that have supplied these invoices in order to classify them according to the field of activity of the company that issued the invoice.

During this project, we have read a lot of documentation, as well as tests on the different possible methods of logo detection on invoices. 

The goal of this project is to classify images by detecting objects. Files can be:
* bill (from serval companies)
* payslip
* account statement

To do so, we used two methods :
- Template matching
- SIFT: Scale Invariant Feature Transform 


This is a student project.
<br></br>


### Built With

* [OpenCV](https://opencv.org/)
* [Pandas](https://pandas.pydata.org/)



<!-- GETTING STARTED -->
## Getting Started

How to install, run and use the project.

### Prerequisites

The project is a Jupyter Notebook. You will have to install the Jupyter Notebook software on your computer. Or, you can install it on AnaConda.

### Installation

_Before compiling one of the two notebook, you will have to check if you have all required Python librairies installed. Otherwise, you will have to install them._

1. Clone the repo
   ```sh
   git clone https://github.com/clementmariebrisson/Finding_Objects_In_Images.git
   ```
2. Open Jupyter Notebook
3. Install Python packages
   ```
    pip install opencv-python
    pip install numpy
    pip install matplotlib
    pip install pdf2image
    pip install Pillow
    pip install regex
    pip install pytesseract
    pip install pandas
   ```

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

We find our scores in a CSV file, which allows us to see the ratio of each logo detection test on a file.
The SIFT Brute Force method is the method that works best among the different ones we tested. Indeed, this method is the most precise and the most adapted to our initial problem.

All methods have their weak points, for SIFT it is the distance of the keypoints that are matched. We were able to overcome this with SIFT - bruteforce, but if the logo does not have much detail, few keypoints are detected and this affects the score calculated by our program.

The bruteforce method was the best way to solve the initial problem, thanks to all the possibilities offered by the knnMatcher.

_For more informations you can read the [report](https://github.com/clementmariebrisson/Finding_Objects_In_Images/blob/main/Rapport.pdf)._

_For more examples, please refer to those sites :_
* [SIFT with python](https://www.analyticsvidhya.com/blog/2019/10/detailed-guide-powerful-sift-technique-image-matching-python)
* [Multi Scale Template Matching with python](https://pyimagesearch.com/2015/01/26/multi-scale-template-matching-using-python-opencv/#download-the-code)

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- CONTACT -->
## Contact

Alexis Guillotin & Clement Marie Brisson

Project Link: [https://github.com/clementmariebrisson/Finding_Objects_In_Images](https://github.com/clementmariebrisson/Finding_Objects_In_Images)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)
* [React Icons](https://react-icons.github.io/react-icons/search)




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/clementmariebrisson/Finding_Objects_In_Images.svg?style=for-the-badge
[contributors-url]: https://github.com/clementmariebrisson/Finding_Objects_In_Images/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/clementmariebrisson/Finding_Objects_In_Images.svg?style=for-the-badge
[forks-url]: https://github.com/clementmariebrisson/Finding_Objects_In_Images/network/members

[stars-shield]: https://img.shields.io/github/stars/clementmariebrisson/Finding_Objects_In_Images.svg?style=for-the-badge
[stars-url]: https://github.com/clementmariebrisson/Finding_Objects_In_Images/stargazers
[issues-shield]: https://img.shields.io/github/issues/clementmariebrisson/Finding_Objects_In_Images.svg?style=for-the-badge
[issues-url]: https://github.com/clementmariebrisson/Finding_Objects_In_Images/issues
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/clementmariebrisson
[product-screenshot]: images/screenshot.png
