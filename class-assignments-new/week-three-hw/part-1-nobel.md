1. find number of winners for each nobel prizes:
chemistry:182
econ:81
literature:114
medicine:216
peace:133
physics:211
2. find winners of multiple Nobel Prize Winners:
tail -n +2 nobel.csv |cut -d "," -f 5-6 | sort -k 6 | uniq -d
"Frederick Sanger
John Bardeen
Linus Carl
marie Curie
 3. Find most common surnames in winners:
tail -n +2 nobel.csv | cut -d "," -f 6 |uniq -d
"Anderson"
"Bardeen"
"Bloch"
"Bohr"
"Bragg"
"Brown"
"Buck"
"Chamberlain"
"Curie
"Fischer"
"Frank"
"Friedman"
"Hall"
"Henderson"
"Hess"
"Hodgkin"
"Hoffmann"
"Jensen"
"Kendall"
"Kornberg"
"Krebs"
"Lee"
"Lewis"
"Marshall"
"Mistral"
"Moser"
"Mott"
"Müller"
"Murad"
"Myrdal"
NA
"Pauling"
"Porter"
"Richards"
"Richardson"
"Sanger"
"Siegbahn"
"Simon"
"Smith"
"Thomson"
"Tinbergen"
"Wiesel"
"Williams"
"Wilson"

Which category has been awarded the most:

tail -n +2 nobel.csv | cut -d "," -f 3 | grep -w cat | wc -l
least: econ
most: medicine
