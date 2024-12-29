# databricks-ai
This project combines Databricks best practices, medallion data architecture, various data sources (including streaming), and an applied use case (financial data) that culminates in training a small LLM. 

# Start project

docker run -it --name databricks-runtime \                                ─╯
  -p 8888:8888 \
  -v ~/databricks-project/data:/mnt/data \
  -v ~/databricks-project/notebooks:/mnt/notebooks \
  databricksruntime/standard:15.4-LTS

  apt-get update

  apt-get install -y python3-pip

  pip3 install jupyter

  jupyter notebook --allow-root --ip=0.0.0.0 --port=8888 --no-browser