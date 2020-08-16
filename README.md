# Co-localization of HP1 isoforms and H3K9me3 in neural stem cells using NGS 

A streamlined pipeline created for the analysis of Cut&Run data

## Getting Strated

### Program Description

H3K9me3 and HP1 isoform signals are processed using Snakemake to inspect their abundancy, co-localization, and potential redundancy. The files containing the results of the analysis are then processed in R to extract further information.

### Installing

The Snakefile along with all scripts and configuration files are ready for download 

## Built With

### Snakemake (v. 5.2.4)

* FastQC (v. 0.11.8)
* MultiQC (v. 1.2)
* Bowtie (v. 2.3.4.2)
* Samtools (v 1.9)
* bamCoverage (v. __)
* SEACR (v. 1.3)
* SEACR_R (v. 1.3) 
* BEDTools (v. 2.26.0)
* DeepTools (v. 2.5.4)
  
### R (v. 4.0.0)
* Data parsing and visualization script

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
