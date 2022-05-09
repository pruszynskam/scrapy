# Scraping OLX site using scrapy

Repository includes 2 python files. The first one - spider_links.py creates a csv file with links to rental offers. The second one - spider2.py generates a dataset that contains detailed info on 100 offers.

In order to get the information on flats offered, one needs to download both spiders from a scrapy project folder. The next step is going to command prompt, making sure that you are in a folder, where all of the spiders downloaded are and type:

### scrapy runspider spider_links.py -s USER_AGENT="custom_user" -o links.csv

that should generate links.csv file in the same folder you and spiders are in. The last step should be going back to your command prompt and typing:

### scrapy runspider spider2.py -s USER_AGENT="custom_user" -o final_data.csv

The final dataset should appear in your folder.
