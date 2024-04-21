# Executive Summary
This project investigates the application of a machine learning model, specifically the T5 transformer, to automatically generate SQL queries from Google's rising search terms expressed in natural language, tailored specifically for non-technical marketers. To demonstrate the feasibility of deploying such technology on accessible hardware, the model was trained and evaluated on my standard laptop using a subset of available data—5,000 training queries and 1,500 test queries selected randomly from the larger WikiSQL dataset, which contains over 56,000 entries. My initial results indicate that while the T5 model can translate natural language into SQL, achieving an exact match in SQL syntax remains a challenge, with a current accuracy of 14%. These findings highlight the potential of machine learning to automate data query generation and emphasize the need for further model optimization and training to enhance accuracy and usability for marketing professionals.

# Rationale
The ability to automatically generate SQL queries from natural language is transformative, especially for marketers who frequently rely on data insights to make informed decisions but may lack technical expertise in SQL. By simplifying the process of extracting actionable information from databases, this technology can significantly enhance the efficiency and effectiveness of marketing strategies. As data becomes increasingly central to competitive advantage, the need for accessible tools that can bridge the gap between complex data queries and strategic decision-making grows. Automating SQL query generation from natural language empowers marketers to leverage data independently, speeding up their response to market trends and improving their capacity to execute data-driven campaigns.

# Research Question
Can a T5 transformer-based model effectively generate correct SQL queries from natural language descriptions, and what level of accuracy can be achieved?

# Data Sources
For this project, I utilized the WikiSQL dataset, a publicly available resource consisting of over 56,000 paired English language questions and their corresponding SQL queries. This dataset is specifically designed to train and evaluate natural language to SQL conversion models and is widely recognized in the machine learning community for its applicability in benchmarking the performance of such models. Additionally, I employed transformer-based models from Hugging Face, a leading repository of state-of-the-art pre-trained models, which provided the foundational architecture (T5 transformer) for this project. The combination of the WikiSQL dataset and Hugging Face's advanced machine learning models enabled a robust framework for tackling the challenge of translating natural language queries into executable SQL statements.

# Results
The model, implemented on a standard laptop using a T5-small configuration from Hugging Face, achieved a 14% accuracy rate in generating exact SQL queries from natural language. This level of accuracy, while initially modest, highlights the potential of the approach under constrained resources. The T5-small model was selected to ensure the project was feasible on minimal hardware, simulating conditions that non-technical marketers might typically experience. Despite these limitations, the model demonstrated the capability to automate SQL query generation, a process traditionally requiring significant technical expertise.

Given the resource constraints—both in terms of computing power and the size of the dataset used for training (only 5,000 out of over 56,000 available records)—these results are promising. They suggest that with further tuning of the model parameters, expansion of the training dataset, and possibly the deployment of more powerful hardware or larger model architectures, there is substantial room for improvement. Enhancing these factors could significantly increase accuracy and make the solution more viable for practical applications, especially for marketers seeking to leverage data-driven insights without deep technical knowledge of databases.

# Next Steps
Future work will focus on expanding the training dataset, implementing more sophisticated data preprocessing techniques, and exploring alternative model architectures or ensemble methods to enhance accuracy.

**Note on Importing Libraries:**
Throughout this Jupyter notebook, libraries are imported as needed within individual cells to maintain clean and efficient code execution. This approach is intentional to accommodate the varied computational demands of each step and to optimize the use of resources on the laptop used for model development and training.

**Note on Model Reference:**
For detailed information on the T5-small model and its fine-tuning process for the SQL query generation task, please refer to the Hugging Face model repository at [this link](https://huggingface.co/mrm8488/t5-small-finetuned-wikiSQL). This repository provides insights into the model architecture and fine-tuning techniques applicable for similar natural language processing tasks.
