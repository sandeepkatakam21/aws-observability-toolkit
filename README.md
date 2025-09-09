# AWS Observability Toolkit

## Overview

The AWS Observability Toolkit is a comprehensive collection of monitoring, alerting, and observability solutions for AWS cloud infrastructure. This toolkit provides pre-built scripts, dashboards, and integrations to help you monitor your AWS resources effectively using industry-standard tools like CloudWatch, OpenSearch, Datadog, and Prometheus.

Whether you're running EC2 instances, Lambda functions, or RDS databases, this toolkit provides the essential monitoring components to ensure your applications are running smoothly and efficiently.

## Features

### 🔍 **AWS CloudWatch Integration**
- Custom CloudWatch dashboards and widgets
- Automated metric collection and alerting
- Log aggregation and analysis
- Cost optimization monitoring

### 🔎 **OpenSearch Integration**
- Pre-built dashboards for AWS services
- Log parsing and visualization
- Advanced search and analytics
- Real-time monitoring capabilities

### 📊 **Datadog Integration**
- AWS service monitoring and metrics
- Infrastructure and application performance monitoring
- Custom dashboards and alerts
- Integration with AWS services

### 📈 **Prometheus Integration**
- Metrics collection and storage
- Alerting rules for AWS resources
- Grafana dashboard templates
- Custom exporters for AWS services

## Directory Structure

```
aws-observability-toolkit/
├── README.md
├── cloudwatch-scripts/          # CloudWatch automation scripts and templates
├── opensearch-dashboards/       # OpenSearch dashboard configurations
├── datadog-integration/         # Datadog monitoring setup and configs
└── prometheus-alerts/           # Prometheus rules and alert configurations
```

## Example Directories

### `/cloudwatch-scripts`
Contains CloudWatch-related automation scripts, dashboard templates, and alarm configurations for various AWS services.

### `/opensearch-dashboards`
Pre-built OpenSearch dashboards for monitoring AWS services, including visualization templates and index patterns.

### `/datadog-integration`
Datadog integration scripts, dashboard templates, and monitoring configurations for AWS infrastructure.

### `/prometheus-alerts`
Prometheus alerting rules, recording rules, and configuration files for monitoring AWS resources.

## Sample Usage

### Monitoring EC2 Instances

```bash
# Deploy CloudWatch monitoring for EC2
./cloudwatch-scripts/setup-ec2-monitoring.sh

# Set up Datadog agent on EC2
./datadog-integration/install-datadog-ec2.sh

# Configure Prometheus Node Exporter
./prometheus-alerts/setup-node-exporter.sh
```

### Monitoring AWS Lambda Functions

```bash
# Enable CloudWatch Insights for Lambda
./cloudwatch-scripts/lambda-insights-setup.sh

# Configure Datadog Lambda monitoring
./datadog-integration/lambda-monitoring-setup.sh

# Set up custom Prometheus metrics for Lambda
./prometheus-alerts/lambda-metrics-config.yaml
```

### Monitoring Amazon RDS

```bash
# Deploy RDS CloudWatch dashboards
./cloudwatch-scripts/rds-dashboard-template.json

# Configure OpenSearch for RDS log analysis
./opensearch-dashboards/rds-logs-dashboard.json

# Set up Datadog RDS monitoring
./datadog-integration/rds-monitoring.yaml

# Configure Prometheus RDS Exporter
./prometheus-alerts/rds-exporter-config.yml
```

## Getting Started

### Prerequisites

- AWS CLI configured with appropriate permissions
- Python 3.8+ (for script execution)
- Docker (for containerized monitoring tools)
- Access to your chosen monitoring platform (Datadog, Prometheus, etc.)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/sandeepkatakam21/aws-observability-toolkit.git
   cd aws-observability-toolkit
   ```

2. **Configure AWS credentials:**
   ```bash
   aws configure
   ```

3. **Choose your monitoring stack:**
   - For CloudWatch: Navigate to `./cloudwatch-scripts/`
   - For OpenSearch: Navigate to `./opensearch-dashboards/`
   - For Datadog: Navigate to `./datadog-integration/`
   - For Prometheus: Navigate to `./prometheus-alerts/`

4. **Follow the specific setup instructions in each directory's README.**

### Quick Start

```bash
# Make scripts executable
find . -name "*.sh" -exec chmod +x {} \;

# Run the setup wizard (coming soon)
./setup-wizard.sh
```

## Configuration

Each monitoring tool has its own configuration requirements:

- **CloudWatch**: Requires appropriate IAM permissions for metric access
- **OpenSearch**: Requires OpenSearch cluster endpoint and authentication
- **Datadog**: Requires Datadog API key and application key
- **Prometheus**: Requires Prometheus server configuration

Refer to each directory's documentation for detailed configuration steps.

## Contributing

We welcome contributions to the AWS Observability Toolkit! Here's how you can help:

### How to Contribute

1. **Fork the repository**
2. **Create a feature branch:**
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes and commit:**
   ```bash
   git commit -m "Add your feature description"
   ```
4. **Push to your branch:**
   ```bash
   git push origin feature/your-feature-name
   ```
5. **Create a Pull Request**

### Contribution Guidelines

- Follow existing code style and conventions
- Add tests for new features
- Update documentation as needed
- Ensure all scripts are tested in a safe environment
- Include example usage in your contributions

### Areas for Contribution

- Additional AWS service monitoring templates
- Enhanced dashboard configurations
- Automation scripts for deployment
- Documentation improvements
- Bug fixes and performance optimizations

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### MIT License Summary

- ✅ Commercial use
- ✅ Modification
- ✅ Distribution
- ✅ Private use
- ❌ Liability
- ❌ Warranty

## Support

For support and questions:

- 📧 Open an issue in this repository
- 📖 Check the documentation in each directory
- 💬 Join our community discussions

## Roadmap

- [ ] Add Terraform modules for infrastructure as code
- [ ] Implement automated testing pipeline
- [ ] Add support for additional AWS services
- [ ] Create interactive setup wizard
- [ ] Add cost optimization monitoring
- [ ] Implement anomaly detection capabilities

---

**Made with ❤️ for the AWS community**
