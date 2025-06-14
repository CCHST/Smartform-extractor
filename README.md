# SmartForm Extractor

**SmartForm Extractor** is a Python-based utility designed to parse Supplier Change Order forms in `.docx` format and extract structured field definitions for downstream processing, automation, or integration (e.g., with Smartsheet).

---

## 📋 Instructions

1. **Get Smartsheet API Key**  
   - Go to your Smartsheet account → **Personal Settings** → **API Access**
   - Generate and save your API token securely

2. **Upload the Word Document**
   - Visit [Claude.ai](https://claude.ai/new)
   - Upload your Supplier Change Order `.docx` file
   - Use Claude to extract form fields in the Python format below

3. **Paste the Extracted Function into the Notebook**  
   - Scroll to the notebook section labeled **"AI generated – paste your own code here"**
   - Replace the placeholder `def parse_supplier_change_order(): ...` with your full function
   - 👉 *Paste it directly into that cell*

4. **Run the Notebook**
   - Press the `Run All` button in the Jupyter Notebook
   - This will parse and return a list of form field dictionaries

---

## 🧠 Function Format Example

Below is the expected Python function format that should be pasted into the notebook:

<details>
<summary>Click to expand</summary>

```python
def parse_supplier_change_order():
    """
    Clean parser for the Supplier Change Order form fields.
    Returns a list of form fields with their types and options.
    """
    form_fields = []

    # Example field
    form_fields.extend([
        {
            "field_name": "Type of Change",
            "type": "dropdown",
            "options": ["New Supplier", "Re-classification", "Remove Supplier", "Administrative Change"]
        },
        {
            "field_name": "Reason for Change",
            "type": "text",
            "options": None
        },
        ...
    ])

    return form_fields
