# ⚡ Function Tools

Function tools are **custom Python functions** that you create and integrate into your agents. This is the most flexible and commonly used approach for adding specific capabilities to your agents.

## 🎯 What You'll Learn

- **Function Tool Creation**: Build custom Python functions as tools
- **Tool Registration**: How to register functions with your agent
- **Parameter Handling**: Managing tool inputs and outputs
- **Error Handling**: Robust error management in tools
- **Best Practices**: Design patterns for effective function tools

## 🧠 Core Concept: Function Tools

Function tools are **Python functions with special characteristics**:
- **Descriptive docstrings**: Help the agent understand when to use them
- **Type annotations**: Clear input/output specifications
- **Return dictionaries**: Structured, informative responses
- **Error handling**: Graceful failure management

#

## Key Advantages
- ✅ **Maximum Flexibility**: Create any functionality you need
- ✅ **Easy Integration**: Simple Python functions
- ✅ **Full Control**: Complete control over behavior
- ✅ **Debugging**: Easy to test and debug

## 🔧 Function Tool Requirements

#

## 1. **Descriptive Docstrings**
```python
def calculate_compound_interest(principal: float, rate: float, years: int) -> dict:
    """
    Calculate compound interest for an investment.
    
    Use this function when users ask about investment growth,
    compound interest calculations, or future value of investments.
    
    Args:
        principal: Initial investment amount
        rate: Annual interest rate (as decimal, e.g., 0.05 for 5%)
        years: Number of years to compound
    
    Returns:
        Dictionary with calculation results and breakdown
    """
```

#

## 2. **Type Annotations**
- Always specify parameter types
- Include return type annotations
- Use appropriate Python types (str, int, float, dict, list)

#

## 3. **Structured Returns**
```python
return {
    "result": final_amount,
    "calculation_breakdown": {
        "principal": principal,
        "rate": rate,
        "years": years,
        "total_interest": total_interest
    },
    "status": "success"
}
```

#

## 4. **Error Handling**
```python
try:
    # Tool logic here
    return {"result": result, "status": "success"}
except ValueError as e:
    return {"error": str(e), "status": "error"}
```

## 🚀 Tutorial Examples

This sub-example includes two practical implementations:

#

## 📍 **Calculator Agent**
**Location**: `./calculator_agent/`
- **Mathematical Operations**: Basic arithmetic, compound interest, percentage calculations
- **Unit Conversions**: Temperature conversions (Celsius, Fahrenheit, Kelvin)
- **Statistical Analysis**: Mean, median, mode, standard deviation for data sets
- **Financial Calculations**: Investment growth, compound interest projections
- **Number Utilities**: Rounding, formatting, and mathematical expressions

#

## 📍 **Utility Agent**
**Location**: `./utility_agent/`
- **Text Processing**: Word counting, case conversions, text transformations
- **Data Extraction**: Email and URL extraction, word frequency analysis
- **Date/Time Operations**: Format conversions, date differences, age calculations
- **Data Utilities**: UUID generation, text hashing, Base64 encoding/decoding
- **Validation Tools**: URL validation, JSON formatting and validation

## 📁 Project Structure

```
4_2_function_tools/
├── README.md                    # This file - function tools guide
├── requirements.txt             # Dependencies for function tools
├── .env.example                # Environment variables template (shared)
├── calculator_agent/           # Mathematical tools implementation
│   ├── __init__.py
│   ├── agent.py               # Calculator agent with custom tools
│   └── tools.py               # Mathematical function tools
└── utility_agent/              # Utility tools implementation
    ├── __init__.py
    ├── agent.py               # Utility agent with various tools
    └── tools.py               # Text processing, date/time, and data utilities
```

## 🎯 Learning Objectives

By the end of this sub-example, you'll understand:
- ✅ How to create custom Python functions as tools
- ✅ Best practices for tool design and documentation
- ✅ How to handle parameters and return values effectively
- ✅ Error handling and validation strategies
- ✅ When to use function tools vs other approaches

## 🚀 Getting Started

1. **Set up your environment**:
   ```bash
   cd 4_2_function_tools
   
   # Copy the environment template
   cp env.example .env
   
   # Edit .env and add your Google AI API key
   # Get your API key from: https://aistudio.google.com/
   ```

2. **Install dependencies**:
   ```bash
   # Install required packages
   pip install -r requirements.txt
   ```

3. **Run the agents**:
   ```bash
   # Start the ADK web interface
   adk web
   
   # In the web interface, select:
   # - calculator_agent: For mathematical calculations and conversions
   # - utility_agent: For text processing, date/time, and data utilities
   ```

4. **Try the agents**:
   - **Calculator Agent**: "Calculate 15% of 200", "Convert 100°F to Celsius", "Find statistics for [1,2,3,4,5]"
   - **Utility Agent**: "Count words in this text", "Format date 2023-12-25", "Generate a UUID"

5. **Create Your Own**: Build custom tools for your use case

## 💡 Pro Tips

- **One Purpose Per Tool**: Each function should do one thing well
- **Rich Docstrings**: The docstring is crucial for agent understanding
- **Validate Inputs**: Always validate function parameters
- **Return Dictionaries**: Structured returns are easier to work with
- **Test Independently**: Test tools outside the agent first

## 🔧 Common Function Tool Patterns

#

## 1. **Simple Calculator Pattern**
```python
def add_numbers(a: float, b: float) -> dict:
    """Add two numbers together."""
    return {"result": a + b, "operation": "addition"}
```

#

## 2. **Data Processing Pattern**
```python
def analyze_text(text: str) -> dict:
    """Analyze text for word count, sentiment, etc."""
    return {
        "word_count": len(text.split()),
        "character_count": len(text),
        "sentiment": "neutral"  # Placeholder
    }
```

#

## 3. **API Integration Pattern**
```python
def get_weather(city: str) -> dict:
    """Get weather information for a city."""
    try:
        # API call logic here
        return {"temperature": 72, "condition": "sunny"}
    except Exception as e:
        return {"error": str(e), "status": "failed"}
```

#

## 4. **Conversion Pattern**
```python
def convert_temperature(temp: float, from_unit: str, to_unit: str) -> dict:
    """Convert temperature between units."""
    # Conversion logic
    return {
        "original": {"value": temp, "unit": from_unit},
        "converted": {"value": converted_temp, "unit": to_unit}
    }
```

## 🚨 Important Notes

- **No Default Parameters**: ADK doesn't support default parameters
- **Return Dictionaries**: Always return structured data
- **Error Handling**: Implement proper error handling
- **Documentation**: Write clear, helpful docstrings
- **Testing**: Test functions independently before adding to agent

## 🔧 Common Use Cases

#

## Mathematical Tools (Calculator Agent)
- Basic arithmetic operations and expressions
- Statistical calculations (mean, median, mode, standard deviation)
- Financial calculations (compound interest, percentages)
- Unit conversions (temperature, measurements)
- Number formatting and rounding

#

## Text Processing Tools (Utility Agent)
- Word and character counting
- Case conversions and text transformations
- Email and URL extraction from text
- Word frequency analysis
- String manipulation and formatting

#

## Date/Time Tools (Utility Agent)
- Date format conversions
- Age calculations and date differences
- Time zone handling
- Duration calculations
- Date parsing and validation

#

## Data Utilities (Utility Agent)
- UUID generation for unique identifiers
- Text hashing with various algorithms
- Base64 encoding and decoding
- URL validation and parsing
- JSON formatting and validation

#

## Integration Tools
- API calls and external service integration
- Database queries and data retrieval
- File operations and data processing
- Custom business logic implementation

## 🛠️ Tech Stack


## 🚀 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
   cd ./ai_agent_framework_crash_course/google_adk_crash_course/4_tool_using_agent/4_2_function_tools
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
