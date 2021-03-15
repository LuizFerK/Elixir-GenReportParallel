<br />

<p align="center">
  <img alt="Logo" src="https://elixir-lang.org/images/logo/logo.png" width="400px" />
</p>

<h1 align="center" style="text-align: center;">Report Generator</h1>

<p align="center">
	<a href="https://github.com/LuizFerK">
		<img alt="Author" src="https://img.shields.io/badge/author-Luiz%20Fernando-FF872C?style=flat" />
	</a>
	<a href="#">
		<img alt="Languages" src="https://img.shields.io/github/languages/count/LuizFerK/Elixir-GenReportParallel?color=%23FF872C&style=flat-" />
	</a>
	<a href="hhttps://github.com/LuizFerK/GoRestaurant/stargazers">
		<img alt="Stars" src="https://img.shields.io/github/stars/LuizFerK/Elixir-GenReportParallel?color=FF872C&style=flat" />
	</a>
	<a href="https://github.com/LuizFerK/GoRestaurant/network/members">
		<img alt="Forks" src="https://img.shields.io/github/forks/LuizFerK/Elixir-GenReportParallel?color=%23FF872C&style=flat" />
	</a>
	<a href="https://github.com/LuizFerK/GoRestaurant/graphs/contributors">
		<img alt="Contributors" src="https://img.shields.io/github/contributors/LuizFerK/Elixir-GenReportParallel?color=FF872C&style=flat" />
	</a>
</p>

<p align="center">
	<b>Freelancers reports!</b><br />
  A simple report generation automation for a company that hired several freelancers!<br />
	<span>Created only with Elixir.</span><br />
	<sub>Made with ❤️</sub>
</p>

<br />

# :pushpin: Contents

- [Features](#rocket-features)
- [Installation](#wrench-installation)
- [Getting started](#bulb-getting-started)
- [Techs](#fire-techs)
- [Issues](#bug-issues)
- [License](#book-license)

# :rocket: Features

- Report generation from a data file with 30 thousand lines
- Generation of the same report but using parallelism with 3 files of 10 thousand lines

# :wrench: Installation

### Required :warning:
- Elixir
- Erlang

### SSH

SSH URLs provide access to a Git repository via SSH, a secure protocol. If you have an SSH key registered in your GitHub account, clone the project using this command:

```git clone git@github.com:LuizFerK/Elixir-GenReportParallel.git```

### HTTPS

In case you don't have an SSH key on your GitHub account, you can clone the project using the HTTPS URL, run this command:

```git clone https://github.com/LuizFerK/Elixir-GenReportParallel.git```

**Both of this commands will generates a folder called Elixir-GenReportParallel, with all the project**

# :bulb: Getting started

1. This project does not have a server, in this case, the mode of use is through IEx (Elixir's interactive shell), which can be accessed using the command ```iex -S mix``` in the project folder;
2. Within IEx, you have two usage options: standard execution (which will run 30 thousand lines in just one process) and parallel execution (which will run 3 files of 10,000 lines simultaneously). To use the standard mode, run the following command:
> ```GenReport.build("gen_report.csv")```
3. If you want to use the parallel mode, run the following command:
> ```GenReport.build_from_many(["gen_report_1.csv", "gen_report_2.csv", "gen_report_3.csv"])```
4. In both modes, you will have the same result, however, parallel execution will be faster;
5. The result structure will be a **map** with the following information: ```all_hours``` (representing the total hours of all developers in the project),```hours_per_month``` (representing the total hours of each developer in all months of the year) and ```hours_per_year``` (representing the total hours of all developers between the years 2016 and 2020).

# :fire: Techs

### Elixir

# :bug: Issues

Find a bug or error on the project? Please, feel free to send me the issue on the [Elixir-GenReportParallel issues area](https://github.com/LuizFerK/Elixir-GenReportParallel/issues), with a title and a description of your found!

If you know the origin of the error and know how to resolve it, please, send me a pull request, I will love to review it!

# :book: License

Released in 2020.

This project is under the [MIT license](https://github.com/LuizFerK/Elixir-GenReportParallel/blob/master/LICENSE).

<p align="center">
	< keep coding /> :rocket: :heart:
</p>
