# How to Open Science: Promoting Principles and Reproducibility Practices within the Learning @ Scale Community

[![OSF][badge]][osf]

*How to Open Science: Promoting Principles and Reproducibility Practices within the Learning @ Scale Community* is a tutorial to be presented at the [*10th ACM Conference on Learning @ Scale*][lats].

This project serves as the repository holding the webpage. The rendered version can be viewed at https://lats2023-tutorial.howtoopenscience.com.

## License

The content of this Open Science Framework project is under the [Creative Commons Attribute 4.0 International License][cc4].

## Local Setup

### [Docker][docker] Container

Clone this repository and run the following commands:

```
docker build -t <image_name> .
docker run --rm -it -p 8000:8000 -v ${PWD}/src:/docs <image_name>
```

`image_name` can be specified to whatever identifier the user desires. This will run the docs server and expose it to the local host on port 8000.

### Python

This setup runs in Python 3.9.5. You can install the required libraries through the provided `requirements.txt`:

```
pip install -r requirements.txt
```

Then navigate to the  `src` folder in your terminal and serve the docs.

```
cd ./src
mkdocs serve
```

> You may need to prefix the `pip` or `mkdocs` command with either `python3 -m` for Unix systems or `py -m` for Windows systems if the python modules were not properly installed onto the path.

## Citation

```
@misc{Haim_Shaw_Heffernan_2023,
  title={How to Open Science: Promoting Principles and Reproducibility Practices within the Learning @ Scale Community},
  url={osf.io/jp6cq},
  DOI={10.17605/OSF.IO/JP6CQ},
  publisher={OSF},
  author={Haim, Aaron and Shaw, Stacy T and Heffernan, Neil T, III},
  year={2023},
  month={Apr}
}
```

[badge]: https://img.shields.io/badge/OSF-10.17605%2Fosf.io%2Fjp6cq-blue
<!-- TODO: Replace with DOI when working -->
[osf]: https://osf.io/jp6cq

[lats]: https://learningatscale.acm.org/las2023/

[cc4]: ./LICENSE

[docker]: https://www.docker.com/
