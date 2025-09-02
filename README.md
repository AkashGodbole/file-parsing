# Complete List of File Parsing Interview Questions

## Coding Problems

### Beginner Level Problems

#### 1. CSV Parser with Error Handling
**Description:** Write a function that parses a CSV file and handles quotes, escaped characters, and different delimiters
**Example Input:** `name,age,"city,state"\nJohn,25,"New York, NY"\nJane,30,Boston`
**Requirements:**
- Handle quoted fields
- Support custom delimiters  
- Handle malformed rows

#### 2. Log File IP Extractor
**Description:** Parse Apache access logs and extract unique IP addresses with their request counts
**Example Input:** `192.168.1.1 - - [10/Oct/2000:13:55:36 -0700] "GET /index.html HTTP/1.0" 200 2326`
**Requirements:**
- Extract IP addresses
- Count occurrences
- Handle malformed log entries

#### 3. Configuration File Parser
**Description:** Parse INI-style configuration files into a nested dictionary structure
**Example Input:** `[database]\nhost=localhost\nport=5432\n[cache]\nttl=3600`
**Requirements:**
- Handle sections
- Parse key-value pairs
- Support comments

#### 4. JSON Flattener
**Description:** Flatten nested JSON objects into a single level with dot notation keys
**Example Input:** `{"user": {"name": "John", "address": {"city": "NYC"}}}`
**Requirements:**
- Handle nested objects
- Handle arrays
- Preserve data types

### Intermediate Level Problems

#### 5. XML to JSON Converter
**Description:** Convert XML documents to JSON while preserving structure and handling attributes
**Example Input:** `<person id="1"><name>John</name><age>25</age></person>`
**Requirements:**
- Handle attributes
- Handle CDATA
- Handle namespaces
- Memory efficient for large files

#### 6. Log Aggregator with Time Windows
**Description:** Parse log files and aggregate events by time windows (e.g., per minute/hour)
**Example Input:** Multiple log files with timestamps and event types
**Requirements:**
- Parse timestamps
- Group by time windows
- Handle multiple log formats
- Memory efficient

#### 7. Protocol Buffer Parser
**Description:** Parse binary protocol buffer messages and convert to readable format
**Example Input:** Binary protobuf data with known schema
**Requirements:**
- Handle different field types
- Handle repeated fields
- Handle nested messages

#### 8. HTML Table Extractor
**Description:** Extract data from HTML tables, handling colspan, rowspan, and nested tables
**Example Input:** HTML page with complex table structures
**Requirements:**
- Handle table headers
- Handle spanning cells
- Handle nested tables
- Output as CSV/JSON

#### 9. YAML Schema Validator
**Description:** Parse YAML files and validate against a predefined schema
**Example Input:** YAML configuration file with validation rules
**Requirements:**
- Parse YAML
- Validate data types
- Check required fields
- Provide meaningful error messages

### Advanced Level Problems

#### 10. Streaming Large File Parser
**Description:** Parse CSV files larger than available memory using streaming/chunking
**Example Input:** Multi-GB CSV files
**Requirements:**
- Constant memory usage
- Handle file chunks
- Resume interrupted parsing
- Progress reporting

#### 11. Multi-format File Detector and Parser
**Description:** Automatically detect file format and parse accordingly (JSON, XML, CSV, etc.)
**Example Input:** Files with unknown formats
**Requirements:**
- Auto-detect format
- Parse multiple formats
- Handle hybrid formats
- Extensible architecture

#### 12. Expression Parser and Evaluator
**Description:** Build a parser for mathematical expressions with variables and functions
**Example Input:** `sin(x) + log(y * 2) where x=1.5, y=10`
**Requirements:**
- Handle operator precedence
- Support functions
- Handle variables
- Error reporting

#### 13. Network Packet Parser
**Description:** Parse network packet captures (PCAP) and extract protocol information
**Example Input:** PCAP file with mixed TCP/UDP traffic
**Requirements:**
- Parse packet headers
- Handle different protocols
- Extract payload
- Performance optimization

#### 14. SQL Query Parser
**Description:** Parse SQL SELECT statements and build an AST (Abstract Syntax Tree)
**Example Input:** `SELECT name, age FROM users WHERE age > 25 ORDER BY name`
**Requirements:**
- Handle SQL syntax
- Build AST
- Validate syntax
- Handle subqueries

#### 15. Diff Parser and Merger
**Description:** Parse unified diff format and apply patches to files
**Example Input:** Git-style diff files with additions/deletions
**Requirements:**
- Parse diff format
- Apply patches
- Handle conflicts
- Generate diffs

### System Design Level Problems

#### 16. Distributed Log Processing System
**Description:** Design a system to parse and process logs from multiple servers
**Requirements:**
- Handle multiple log formats
- Scale to millions of log entries per second
- Real-time processing and alerting
- Fault tolerance and recovery
- Data partitioning and distribution

#### 17. File Format Translation Service
**Description:** Design a service that converts between different file formats (CSV, JSON, XML, Parquet)
**Requirements:**
- Support multiple input/output formats
- Handle large files (streaming)
- Schema mapping and validation
- Rate limiting and quotas
- Async processing with job queues

#### 18. Real-time Data Pipeline Parser
**Description:** Design a real-time parsing system for streaming data (Kafka, Kinesis)
**Requirements:**
- Handle multiple data formats
- Real-time processing with low latency
- Schema evolution handling
- Dead letter queues for failed parsing
- Monitoring and alerting
