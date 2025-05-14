
# Email Verifer tool



A simple Go program that checks whether a given domain supports email by verifying the presence of MX, SPF, and DMARC DNS records.

Features

**MX Record Check** – Verifies if the domain has Mail Exchange records.

**SPF Record Check** – Looks for v=spf1 TXT records to confirm SPF configuration.

**DMARC Record Check** – Checks _dmarc.domain for v=DMARC1 records

## How to Use

### 1. Build the Program

```bash
go build -o email-verifier main.go
```

### 2. Run the Program

You can either:
- Run and type domain names manually
- Pipe in a file of domains

#### Option 1: Manual Input

```bash
./email-verifier
example.com
google.com
<Ctrl+D>  To end input on Unix/macOS; use Ctrl+Z on Windows
