# DNSIntel

Modular DNS reconnaissance and analysis engine designed to extract structured intelligence from domain infrastructure.

---

## Features

- DNS record collection (A, MX, NS, TXT, PTR)
- Subdomain enumeration (wordlist-based)
- SPF / DMARC analysis
- MX infrastructure expansion
- Basic takeover heuristics
- Structured JSON output

---

## Architecture

Collector → Analyzer → Output

- collector/ → gathers raw DNS data  
- analyzer/ → extracts security signals  
- utils/ → shared logic (resolver, HTTP)  
- data/ → raw + analyzed output  

---

## Usage

python3 main.py example.com

---

## Output

data/raw/example.json  
data/analyzed/example_analysis.json  

---

## Roadmap

- [ ] DNS diff tracking  
- [ ] Takeover fingerprinting  
- [ ] CLI flags (--deep, --fast)  
- [ ] Parallel scanning  

---

## License

MIT License
