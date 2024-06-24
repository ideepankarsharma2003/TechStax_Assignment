# **TechSta`X` Assignment**
---
### Steps to setup the project
1. Expose the flask endpoint in the `webhooks`.

![alt text](images/image-12.png)

2. Select `Pull-Request` and `Pushes` to setup webhooks.

![alt text](images/image-13.png)

3. Start the flask server.

![alt text](images/image-14.png)

4. In `app/extensions.py` we can comment this line. I only added that because there were so many logs in UI.
```python
mongo = MongoClient('mongodb://localhost:27017/')
db = mongo['webhook_db']
# db.drop_collection("events")
collection = db['events']
```




---
### Screenshots
---
1. `Push`: Removed everything from my repository and made the commit .

![alt text](images/image.png)

![alt text](images/image-1.png)

![alt text](images/image-2.png)

![alt text](images/image-3.png)
---

2. `Pull Request`: Made a pull request from the branch `ideepankarsharma2003-patch-2`.

![alt text](images/image-4.png)

![alt text](images/image-5.png)

![alt text](images/image-6.png)

![alt text](images/image-7.png)
---
3. `Merge`: Merged the branch `ideepankarsharma2003-patch-2` with the `main`.

![alt text](images/image-8.png)

![alt text](images/image-9.png)

![alt text](images/image-10.png)

![alt text](images/image-11.png)