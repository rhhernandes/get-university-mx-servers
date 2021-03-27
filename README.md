# Get US universities mail servers

This [script](get-universities.ipynb) uses Python module `dnspython` to gather information on what email providers are used by each American university.

The full list of universities and their web pages was generated from the [National Center for Education Statistics' Integrated Postsecondary Education Data System](https://nces.ed.gov/ipeds/datacenter/Data.aspx). It was saved to the `.data/in/universities_urls.csv` file.

From the same data system, another table was generated containing the estimated enrollments for undergraduate and graduate students in each institution, `data/in/estimated_enrollment.csv`. This information allos to estimate how many students have their data collected and treated by the tech companies.

This work is partially based on Filipe Saraiva's [research](https://gitlab.com/ccsl-ufpa/get-mx-universities/-/blob/master/get-mx-universities.py) for the Federal University of Pará, in Brazil. It is a simpler version, though, focusing solely on the MX servers used. Also, as stated, it uses the module `dnspython` instead of the `host` command, making this script also compatible with Windows.

Further reference:
* https://www.dnspython.org/
* https://gitlab.com/ccsl-ufpa/get-mx-universities/-/blob/master/get-mx-universities.py
* https://stackoverflow.com/questions/4336849/mx-record-lookup-and-check/4339305
* https://www.exclamationsoft.com/exclamationsoft/netmailbot/help/reference/find_mail_server.asp    

# License

This software is distributed under the [MIT license](LICENSE).