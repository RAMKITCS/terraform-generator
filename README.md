# 🚀 AI-Powered Terraform Code Generator

This project is a powerful Streamlit-based application designed to automatically generate and refine Terraform code using OpenAI's GPT model. It simplifies the creation of modular, best-practice Terraform configurations for AWS, Azure, and GCP services.

## 📋 Features
✅ **Modular Code Generation** — Generates `variables.tf`, `main.tf`, `outputs.tf`, and `instructions.md` for clear and organized Terraform structure.  
✅ **Pre-requisite Option** — Option to include required infrastructure pre-requisites such as VPC, Subnets, NSGs, etc.  
✅ **Refinement Support** — Users can refine generated code using natural language feedback.  
✅ **Custom Services** — Users can add their own custom services via the UI.  
✅ **Downloadable Code Files** — Each file is downloadable separately for improved project structure.  
✅ **Clear Deployment Guidance** — Instructions are provided to ensure seamless deployment of the generated code.  

## 🏗️ Prerequisites
1. **Python 3.10+** installed on your machine.
2. **Terraform** installed for syntax validation and deployment.
3. An **OpenAI API Key** for code generation.

## ⚙️ Setup Instructions
1. **Clone the Repository**
```bash
git clone <repository-url>
cd terraform-code-generator
```

2. **Create a Virtual Environment**
```bash
python -m venv venv
source venv/bin/activate    # Linux/MacOS
venv\Scripts\activate       # Windows
```

3. **Install Dependencies**
```bash
pip install -r requirements.txt
```

4. **Set Up Environment Variables**
Create a `.env` file in the project root and add your OpenAI API key:
```
OPENAI_API_KEY=<YOUR_OPENAI_API_KEY>
```

5. **Run the Application**
```bash
streamlit run iac_cac_generator_1.py
```

## 🚀 How to Use the Application
1. **Select Configuration Options:**
   - Choose your cloud provider (AWS, Azure, GCP).
   - Select your desired service (e.g., EC2, AKS, GKE, etc.).
   - Check the **"Include Pre-requisites"** box if you want pre-requisite infrastructure included.

2. **Generate Configuration:**
   - Click the `Generate Configuration` button to create modular Terraform files.

3. **Refine the Configuration:**
   - Provide natural language feedback in the refinement text box to improve the generated code.

4. **Download Files:**
   - Download individual `.tf` and `.md` files for better project organization.

## 🛡️ Best Practices in Code Generation
The generated Terraform code follows industry best practices:
- Use of **variables** for flexibility.
- Inclusion of **security measures** like security groups, IAM roles, and encryption.
- Proper use of **`depends_on`** for dependencies between resources.

## 🐞 Troubleshooting
✅ **Missing API Key Error:** Ensure you’ve added your OpenAI API Key to the `.env` file.  
✅ **Empty Configuration Output:** Verify your OpenAI API Key is active and check your OpenAI account limits.  
✅ **Code Formatting Issues:** Run `terraform fmt` to auto-format generated Terraform files.  

## 📌 Future Enhancements
🚀 Add Terraform Cloud integration for automatic deployments.  
🚀 Introduce cost estimation guidance for generated resources.  
🚀 Enable visual diagram generation for architecture previews.  

## 🧑‍💻 Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a feature branch.
3. Submit a pull request with your changes.

## 📄 License
This project is licensed under the **MIT License**. Feel free to use and modify it as needed.

---
For further questions or support, feel free to reach out! 😊

