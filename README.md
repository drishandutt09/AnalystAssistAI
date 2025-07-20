# AnalystAssistAI
AnalystAssistAI - An intelligent AI-powered ticketing system that provides automated analysis, recommendations, and multi-channel communication through email and voice calls.
🚀 Overview
The AI Ticketing Assistance System is a comprehensive automation solution built with N8N that intelligently processes support tickets, provides detailed technical analysis, and communicates with analysts through both email reports and AI-powered voice calls. Perfect for IT departments, security teams, and support organizations looking to enhance their incident response capabilities.
✨ Key Features
🤖 Dual AI Agents
•	Email Analysis Agent: Generates comprehensive technical reports for analyst review
•	Voice Calling Agent: Conducts professional phone conversations with detailed explanations
📋 Smart Form Interface
•	User-friendly web form for ticket submission
•	Captures essential information: user details, role, issue description, contact preferences
•	Automatic routing based on communication preference (Email/Phone)
📧 Intelligent Email Analysis
•	Comprehensive technical investigation and root cause analysis
•	Risk assessment and impact evaluation
•	Detailed recommendations with implementation timelines
•	Professional analyst-focused reporting format
📞 AI Voice Communication
•	Professional, friendly AI calling agent named "Tetris - TicketGuard"
•	Adaptive conversation based on user role and issue complexity
•	Real-time ticket explanation and recommendations
•	Integration with Retell AI for natural voice interactions
🔄 Automated Workflows
•	Conditional routing based on user preferences
•	Seamless integration between form submission and response generation
•	Automated follow-up and escalation protocols
🏗️ System Architecture
graph TD
    A[Web Form Submission] --> B{Communication Preference}
    B -->|Email| C[Email Analysis Agent]
    B -->|Phone| D[Voice Calling Agent]
    C --> E[OpenAI GPT-4 Analysis]
    D --> F[OpenAI GPT-4 Conversation]
    E --> G[Gmail Integration]
    F --> H[Retell AI Voice Call]
    G --> I[Detailed Email Report]
    H --> J[Professional Phone Conversation]
🛠️ Technical Stack
•	Automation Platform: N8N
•	AI Language Model: OpenAI GPT-4.1 Mini
•	Voice AI: Retell AI
•	Email Service: Gmail API
•	Form Processing: N8N Form Trigger
•	Data Format: JSON workflow configuration
📦 Installation & Setup
Prerequisites
•	N8N instance (self-hosted or cloud)
•	OpenAI API key with GPT-4 access
•	Retell AI account and API credentials
•	Gmail account with API access enabled
•	Phone number for outbound calling (Retell AI)
Setup Steps
1.	Clone the Repository
2.	git clone https://github.com/yourusername/ai-ticketing-assistance.git
3.	cd ai-ticketing-assistance
4.	Import N8N Workflow
o	Open your N8N instance
o	Go to Workflows → Import from file
o	Upload My_workflow.json
5.	Configure Credentials
o	OpenAI API: Add your OpenAI API key
o	Retell AI: Configure your Retell AI authentication
o	Gmail: Set up Gmail OAuth2 credentials
6.	Update Retell AI Configuration
7.	{
8.	  "from_number": "+15715345089",
9.	  "override_agent_id": "agent_6392077fc531952345256af099"
10.	}
11.	Activate the Workflow
o	Enable the workflow in N8N
o	Test the form trigger endpoint
🔧 Configuration
Form Fields Configuration
The system captures the following information:
Field	Type	Required	Description
User Name	Text	✅	Full name of the user
Mobile Number	Number	✅	Phone number for callbacks
User Role	Text	✅	Job role/position
Ticket Details	Textarea	✅	Comprehensive issue description
Email Address	Email	✅	Contact email
Communication Preference	Dropdown	✅	Email or Telephone
AI Agent Customization
Email Analysis Agent
•	System Role: Technical analysis specialist
•	Focus: Comprehensive investigation and recommendations
•	Output: Structured email reports for analyst review
Voice Calling Agent
•	Personality: Professional, friendly, knowledgeable
•	Name: "Tetris - TicketGuard"
•	Capabilities: Adaptive conversation, role-based communication
•	Features: Issue explanation, recommendations, follow-up support
📝 Usage Examples
Example 1: Security Incident (Phishing Email)
Input:
•	User: Dave (Analyst)
•	Issue: User Alina reported phishing email
•	Preference: Email
Output: Comprehensive email analysis including:
•	Technical breakdown of phishing indicators
•	Risk assessment and impact analysis
•	Immediate action recommendations
•	Long-term prevention strategies
Example 2: IT Issue with Phone Support
Input:
•	User: Sarah (Manager)
•	Issue: System performance degradation
•	Preference: Telephone
Output: Professional AI voice call providing:
•	Clear explanation of the issue
•	Business impact assessment
•	Step-by-step resolution guidance
•	Follow-up scheduling
🎯 Use Cases
•	IT Help Desk: Automated technical analysis and user communication
•	Security Operations: Incident response and threat analysis
•	Customer Support: Intelligent ticket processing and follow-up
•	Service Management: Automated analyst assignment and reporting
🔒 Security & Privacy
•	All API communications are encrypted
•	User data is processed securely within N8N workflows
•	No persistent storage of sensitive information
•	Compliant with data protection standards
📊 Monitoring & Analytics
The system provides insights on:
•	Ticket processing times
•	Communication preference trends
•	Issue category distribution
•	User satisfaction metrics
🤝 Contributing
We welcome contributions! Please follow these steps:
1.	Fork the repository
2.	Create a feature branch (git checkout -b feature/amazing-feature)
3.	Commit your changes (git commit -m 'Add amazing feature')
4.	Push to the branch (git push origin feature/amazing-feature)
5.	Open a Pull Request
📋 Workflow Structure
Nodes Overview
1.	Form Trigger: Captures user submissions
2.	Conditional Router: Routes based on communication preference
3.	Email Analysis Agent: Generates comprehensive reports
4.	Voice Calling Agent: Prepares conversation content
5.	Gmail Integration: Sends detailed email reports
6.	Retell AI Integration: Initiates voice calls
7.	OpenAI Models: Power both AI agents
🔧 Customization Options
Modify AI Personalities
•	Update system prompts in AI Agent nodes
•	Adjust tone, expertise level, and communication style
•	Add industry-specific knowledge and terminology
Extend Form Fields
•	Add custom fields in the Form Trigger node
•	Update AI agents to process additional information
•	Modify email templates and conversation flows
Integration Enhancements
•	Connect to ticketing systems (Jira, ServiceNow)
•	Add Slack/Teams notifications
•	Implement database logging and analytics
📞 Support & Contact
•	Issues: GitHub Issues
•	Discussions: GitHub Discussions
•	Email: drishandutt9@gmail.com
📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
🙏 Acknowledgments
•	N8N Community for the powerful automation platform
•	OpenAI for advanced language model capabilities
•	Retell AI for natural voice interaction technology
•	Contributors who help improve this project
________________________________________
🌟 Star this repository if you find it helpful!
Made with ❤️ for better IT support automation

