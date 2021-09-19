# PyCon India 2021

This repository hosts the slides and examples for PyCon India 2021 talk on "Building Polyglot applications using MetaCall Core". The talk proposal for the conference can be viewed on the [Proposals Page](https://in.pycon.org/cfp/2021/proposals/building-polyglot-python-applications-using-metacall-core~av2QX/) and the schedule can be viewed on the [Schedule Page](https://in.pycon.org/2021/schedule/). The recordings would be soon released.

## Setup

To setup the slides on your local machine, follow these steps:

1. Install  [hugo](https://gohugo.io/getting-started/installing/)
2. For development:

	```sh
	hugo server -D
	```

3. In  `config.toml`  set  `baseURL`  to be the baseURL of your hosted website.
4. To build and serve it using Docker, push the following command:

	```sh
	docker run --rm -it \
	  -v $(pwd):/src \
	  -p 1313:1313 \
	  klakegg/hugo:0.83.1 \
	  server
	```

## Examples

The instructions to run the examples are given in the individual `README.md` for each example. To make sure the examples run, install the MetaCall CLI:

```sh
curl -sL https://raw.githubusercontent.com/metacall/install/master/install.sh | sh
```

- [Calculation Demo](examples/calculation-demo): Example to showcase cross-language function calls between Python and JavaScript.
- [Machine Learning-based News scrapper](examples/ml-news-article-scraper-example): Polyglot Node App using a Python script to scrap similar news articles from all over the Web using Machine Learning.

## Acknowledgements

The slide format is inspired from [Anirudh Dagar's Quansight Labs Internship talk](https://github.com/AnirudhDagar/qs-intern-talk) and [Thomas J. Fan's Hugo+Reveal Slide template](https://github.com/thomasjpfan/slides-template-hugo).
