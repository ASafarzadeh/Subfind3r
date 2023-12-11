<!--[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Subfind3r?style=for-the-badge)
![PyPI - Status](https://img.shields.io/pypi/status/subfind3r?style=for-the-badge)
![PyPI - Version](https://img.shields.io/pypi/v/subfind3r?style=for-the-badge)
<br>-->


<div align="center">
<pre>                                                                                              
 ____        _      __ _           _ _____      
/ ___| _   _| |__  / _(_)_ __   __| |___ / _ __ 
\___ \| | | | '_ \| |_| | '_ \ / _` | |_ \| '__|
 ___) | |_| | |_) |  _| | | | | (_| |___) | |   
|____/ \__,_|_.__/|_| |_|_| |_|\__,_|____/|_|   </pre>
  <h1 align="center">Subfind3r</h1>

  <p align="center">
    An improved version of <a href="https://github.com/aboul3la/Sublist3r">Sublist3r</a>
    <br>
  </p>
</div>



### Quick start
```
pip install subfind3r
```
```
subfind3r -d example.com
```

## About Subfind3r

![ScreenShot](https://github.com/ASafarzadeh/Subfind3r/blob/main/demo.png?raw=true)


Subfind3r is an improved version of [Sublist3r by aboul3la](https://github.com/aboul3la/Sublist3r) Since it has some problems in some of its functionalities, and also to make the chance for community to Contribute to a powerfull and fast Subdomain enumeration tool.


### Installation

Subfind3r can be easily installed by pip using:
```
pip install subfind3r
```
`The pip way is recommended because it adds the script to the path automatically in mac and linux, and installs the needed dependencies automatically`
or you can use it using git clone command:

```
git clone https://github.com/ASafarzadeh/Subfind3r
```
The pip way does all the installations for you, but in the git clone way you should install the dependencies if they arent already installed. Subfind3r depends on `requests`, `dnspython` and `argparse` python modules.<br><br>
You can install them all with the command below:
```
python -m pip install requests dnspython argparse
```
<br>Now you can navigate to Subfind3r directory, and use it as the example below:
```
python subfind3r.py -d example.com
```



<!-- USAGE EXAMPLES -->
## Usage

Short Form    | Long Form     | Description
------------- | ------------- |-------------
-d            | --domain      | Domain name to enumerate subdomains of
-b            | --bruteforce  | Enable the subbrute bruteforce module
-p            | --ports       | Scan the found subdomains against specific tcp ports
-v            | --verbose     | Enable the verbose mode and display results in realtime
-vt           | --vtkey       | Virus Total Api key(Optional)
-t            | --threads     | Number of threads to use for subbrute bruteforce
-e            | --engines     | Specify a comma-separated list of search engines
-o            | --output      | Save the results to text file
-h            | --help        | show the help message and exit

### Examples

* To list all the basic options and switches use -h switch:

```python subfind3r.py -h```

* To enumerate subdomains of specific domain:

``python subfind3r.py -d example.com``

* To enumerate subdomains of specific domain and show only subdomains which have open ports 80 and 443 :

``python subfind3r.py -d example.com -p 80,443``

* To enumerate subdomains of specific domain and show the results in realtime:

``python subfind3r.py -v -d example.com``

* To enumerate subdomains and enable the bruteforce module:

``python subfind3r.py -b -d example.com``

* To enumerate subdomains and use specific engines such Google, Yahoo and Virustotal engines

``python subfind3r.py -e google,yahoo,virustotal -d example.com``

* With any of the examples above, you can add your <a href="https://www.virustotal.com/">Virus Total Api key</a> to enable VirusTotal search

``python subfind3r.py -d example.com -vt <your-apikey>``


<!-- CONTRIBUTING -->
## Contributing

Contributions are one of the main reasons why Subfind3r is born, So Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make Subfind3r better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- LICENSE -->
## License

Subfind3r is Distributed under the GNU GPL license. take a look at the [LICENSE](https://github.com/ASafarzadeh/Subfind3r/blob/master/LICENSE) for more information.


<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Subfind3r is based on the efforts of these cool guys:
* [aboul3la, by creating the Sublist3r](https://github.com/aboul3la/Sublist3r)
* [The Rook, by creating the Subbrute](https://github.com/TheRook/subbrute)


<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/github/contributors/ASafarzadeh/Subfind3r.svg?style=for-the-badge
[contributors-url]: https://github.com/ASafarzadeh/Subfind3r/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/ASafarzadeh/Subfind3r.svg?style=for-the-badge
[forks-url]: https://github.com/ASafarzadeh/Subfind3r/network/members
[stars-shield]: https://img.shields.io/github/stars/ASafarzadeh/Subfind3r.svg?style=for-the-badge
[stars-url]: https://github.com/ASafarzadeh/Subfind3r/stargazers
[issues-shield]: https://img.shields.io/github/issues/ASafarzadeh/Subfind3r.svg?style=for-the-badge
[issues-url]: https://github.com/ASafarzadeh/Subfind3r/issues
[license-shield]: https://img.shields.io/github/license/ASafarzadeh/Subfind3r.svg?style=for-the-badge
[license-url]: https://github.com/ASafarzadeh/Subfind3r/blob/master/LICENSE.txt
