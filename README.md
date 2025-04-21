# gmane-data-ret

📬 Email Data Extraction and Visualization
As part of this project, I explored email data from Dr. Chuck's public mailing list archive hosted at http://mbox.dr-chuck.net/sakai.devel/. I modified the original gmane.py script to include a constant MANY, which allowed me to control the number of emails retrieved — in this case, limited to 100. This was done intentionally to avoid fetching excessive data and getting stuck in a large processing loop.

The retrieved email metadata was stored locally in an SQLite database (content.sqlite). I then established a connection to this database and processed the relevant fields using Pandas for analysis. Finally, I visualized the number of messages sent per day with Matplotlib, as demonstrated in the testing.ipynb notebook.

This approach allowed for efficient extraction, storage, and visualization of real-world email data for analysis and learning purposes.

