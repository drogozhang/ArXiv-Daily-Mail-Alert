# ArXiv-Daily-Mail-Alert

Daily ArXiv paper notification, customized keywords / authors filter.



## Launch

#### Step 1. Requirements

```

feedparser==5.2.1

```



#### Step 2. Set up the config.

In the demo.config, set up the sender, password, and retriever for mail notifications.

More importantly, you can set the keywords, categories, and authors that you want to keep track of.

**keywords**: return paper's **title** OR **abstract** contains at least one keyword of interest

**authors**: return paper's author list contains at least one author of interest

**categories**: return paper at least belongs to one of the named categories



Note that only papers that **met all above three factors** will be returned. Hence, to follow specific authors not limited to any keyword, simply leave the `keywords` list in the config.yaml blank. Similarly, to follow specific topics not limited to any author, leave the `authors` list bank.

So, you can make **two yamls** for separate authors and keywords following.



#### Step 3. Run

```linux
python --config_path [CONFIG_PATH]
```



#### Step 4. Run it Daily

Combined with `crontab`, you will be notified daily.



### Contact

If you have any questions, feel free to contact Kai Zhang `drogozhang@gmail.com` or open an issue, I will solve it as promptly as I can.
