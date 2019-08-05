# DOI-adder
adds doi to .bib files

based on codes written by [XaraB](https://tex.stackexchange.com/users/101368/xarab).

The stack exchange reply can be found [here](https://tex.stackexchange.com/questions/6810/automatically-adding-doi-fields-to-a-hand-made-bibliography).

The requirements are bibtexparser and unidecode.

Using Conda:
first use the .yml file to create an environment:

```
conda env create --file=env.yml
```

After activating the env you can use it as such :

```
python doi_adder.py {bib-file-name}.bib
```

And it will look like this :

```
Reading Bibliography...
Looking for Dois...
161/162 entries processed, please wait...
We added 49 DOIs !
Before: 42/162 entries had DOI
Now: 91/162 entries have DOI
Writing result to  test.bib_doi.bib
```

You can now just check {bib-file-name}.bib_doi.bib.

Happy Latex-ing!
