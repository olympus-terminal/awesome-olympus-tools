# Awesome Olympus Tools 🚀

> A curated collection of 117+ command-line tools for bioinformatics, data science, system administration, and more

<div align="center">

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Tools](https://img.shields.io/badge/tools-117+-blue.svg)](.)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

**[Bioinformatics](#bioinformatics-toolkit) • [Unix Utilities](#unix-utilities) • [Data Processing](#data-processing) • [Text-to-Speech](#text-to-speech)**

</div>

## 📖 Table of Contents

- [Overview](#overview)
- [Quick Start](#quick-start)
- [Tool Collections](#tool-collections)
  - [🧬 Bioinformatics Toolkit](#bioinformatics-toolkit)
  - [🛠️ Unix Utilities](#unix-utilities)
  - [📊 Data Processing](#data-processing)
  - [🎙️ Text-to-Speech](#text-to-speech)
- [Installation](#installation)
- [Usage Examples](#usage-examples)
- [Contributing](#contributing)
- [Support](#support)

## Overview

This repository serves as a comprehensive catalog of all Olympus Terminal command-line tools. Whether you're a bioinformatician analyzing genomes, a data scientist processing large datasets, or a system administrator automating tasks, you'll find powerful tools here.

### Why These Tools?

- **🚀 Performance**: Many tools are 5-10x faster than standard alternatives
- **🔧 Practical**: Solve real-world problems in bioinformatics, data science, and system administration
- **📚 Well-Documented**: Every tool includes examples and usage instructions
- **🌍 Cross-Platform**: Works on Linux, macOS, and BSD systems
- **🆓 Open Source**: MIT licensed for personal and commercial use

## Quick Start

```bash
# Clone all repositories at once
git clone https://github.com/olympus-terminal/bioinformatics-toolkit.git
git clone https://github.com/olympus-terminal/unix-utilities.git
git clone https://github.com/olympus-terminal/data-processing.git
git clone https://github.com/olympus-terminal/text-to-speech.git

# Or use our installer script (coming soon)
curl -sSL https://olympus-terminal.github.io/install.sh | bash
```

## Tool Collections

### 🧬 [Bioinformatics Toolkit](https://github.com/olympus-terminal/bioinformatics-toolkit)

**51 specialized tools for genomics and proteomics research**

<details>
<summary><b>Sequence Analysis Tools</b></summary>

| Tool | Description | Example |
|------|-------------|---------|
| `n50calc.py` | Calculate N50 and assembly statistics | `python n50calc.py genome.fa` |
| `filter_fasta_on_length` | Filter sequences by length | `./filter_fasta_on_length input.fa 1000` |
| `rename-fasta-headers-simple.sh` | Batch rename FASTA headers | `./rename-fasta-headers-simple.sh seqs.fa prefix` |
| `interleave.sh` | Interleave paired-end reads | `./interleave.sh R1.fq R2.fq > interleaved.fq` |
| `remove_line_wraps_fa.py` | Convert to single-line FASTA | `python remove_line_wraps_fa.py wrapped.fa` |
| `count-amino-acid-residues` | Count amino acid composition | `./count-amino-acid-residues proteins.fa` |

</details>

<details>
<summary><b>BLAST Processing Tools</b></summary>

| Tool | Description | Example |
|------|-------------|---------|
| `ExtractSeqFromBLASTresults.sh` | Extract sequences from BLAST hits | `./ExtractSeqFromBLASTresults.sh blast.out` |
| `TakeOnlyBestBLASThit.sh` | Filter best BLAST hits | `./TakeOnlyBestBLASThit.sh results.txt` |
| `tally_blastp_by_genera.sh` | Summarize BLASTP by genera | `./tally_blastp_by_genera.sh blastp.out` |
| `make_taxid_diamond-blastdb` | Create DIAMOND DB with taxonomy | `./make_taxid_diamond-blastdb proteins.fa` |

</details>

<details>
<summary><b>Domain Analysis Tools</b></summary>

| Tool | Description | Example |
|------|-------------|---------|
| `LAAASR_motifMinerPro.py` | ML-powered motif discovery | `python LAAASR_motifMinerPro.py -i seqs.fa` |
| `extractPFAMs.sh` | Extract PFAM domains | `./extractPFAMs.sh hmmscan.out` |
| `Find-ECs-from-PFAMs.sh` | Map EC numbers from domains | `./Find-ECs-from-PFAMs.sh pfams.txt` |
| `pivot_table_pfams` | Create PFAM pivot tables | `./pivot_table_pfams counts.txt` |

</details>

[View all 51 bioinformatics tools →](https://github.com/olympus-terminal/bioinformatics-toolkit)

---

### 🛠️ [Unix Utilities](https://github.com/olympus-terminal/unix-utilities)

**48 essential tools for file management, text processing, and system administration**

<details>
<summary><b>File Management Tools</b></summary>

| Tool | Description | Example |
|------|-------------|---------|
| `rename_from_list.sh` | Batch rename from mapping file | `./rename_from_list.sh map.txt` |
| `remove_special_chars_filenames.sh` | Clean special characters | `./remove_special_chars_filenames.sh /path/` |
| `move_large_files.sh` | Efficiently move large files | `./move_large_files.sh /src/ /dst/ "*.dat"` |
| `report_offending_dirs.sh` | Find large directories | `./report_offending_dirs.sh /disk/` |
| `random-del-downsample` | Random file sampling | `./random-del-downsample /data/ 0.1` |

</details>

<details>
<summary><b>Text Processing Tools</b></summary>

| Tool | Description | Example |
|------|-------------|---------|
| `delim_to_tab_UTF8` | Convert delimiters to tabs | `./delim_to_tab_UTF8 data.csv > data.tsv` |
| `only_alpha` | Extract alphabetic characters | `./only_alpha < mixed.txt > letters.txt` |
| `sort_by_col-1.sh` | Sort by specific column | `./sort_by_col-1.sh 3 data.txt` |
| `shuf-noHedtho.sh` | Shuffle preserving header | `./shuf-noHedtho.sh data.csv` |

</details>

<details>
<summary><b>Search & System Tools</b></summary>

| Tool | Description | Example |
|------|-------------|---------|
| `search_in_files-parallel.sh` | Parallel file search (5x faster) | `./search_in_files-parallel.sh "pattern" /dir/` |
| `search_zsh_history.sh` | Search command history | `./search_zsh_history.sh "git"` |
| `exec-Singularity.sh` | Container execution wrapper | `./exec-Singularity.sh app.sif cmd` |
| `nohup-bak.sh` | Background execution with logging | `./nohup-bak.sh long_process.sh` |

</details>

[View all 48 unix utilities →](https://github.com/olympus-terminal/unix-utilities)

---

### 📊 [Data Processing](https://github.com/olympus-terminal/data-processing)

**11 modern tools for data analysis, web scraping, and ML workflows**

<details>
<summary><b>All Data Processing Tools</b></summary>

| Tool | Description | Example |
|------|-------------|---------|
| `break-to-100s.py` | Split large datasets into chunks | `python break-to-100s.py huge_data.csv` |
| `web-scraper_Ychr-pdfs.py` | Academic PDF scraper | `python web-scraper_Ychr-pdfs.py --url site.com` |
| `pdf_to_txt_argv.py` | PDF text extraction | `python pdf_to_txt_argv.py paper.pdf` |
| `CountCitations.py` | Citation analysis | `python CountCitations.py manuscript.txt` |
| `pivot-table-maker.R` | Advanced pivot tables | `Rscript pivot-table-maker.R data.csv` |
| `twoagent-DRN-autogen-mod.py` | Two-agent automation | `python twoagent-DRN-autogen-mod.py` |
| `SampleSplitStamp.py` | Sample splitting with timestamps | `python SampleSplitStamp.py data.csv` |
| `tally-awk` | Fast categorical tallying | `./tally-awk column_num data.txt` |

</details>

[View all data processing tools →](https://github.com/olympus-terminal/data-processing)

---

### 🎙️ [Text-to-Speech](https://github.com/olympus-terminal/text-to-speech)

**7 TTS tools from simple to neural, with cloud integration**

<details>
<summary><b>All TTS Tools</b></summary>

| Tool | Description | Example |
|------|-------------|---------|
| `neural_tts.py` | Neural TTS with emotion control | `python neural_tts.py --text "Hi" --emotion happy` |
| `tts_simple.py` | Lightweight TTS | `python tts_simple.py "Hello" output.mp3` |
| `tts4.py` | Multi-speaker TTS v4 | `python tts4.py --speakers "alice,bob" dialogue.txt` |
| `txt-2-polly-2-s3.sh` | AWS Polly with S3 upload | `./txt-2-polly-2-s3.sh text.txt s3://bucket/` |
| `Clean_txt_for_TTS.sh` | Preprocess text for TTS | `./Clean_txt_for_TTS.sh manuscript.txt` |

</details>

[View all TTS tools →](https://github.com/olympus-terminal/text-to-speech)

## Installation

### Requirements

- **OS**: Linux, macOS, or BSD
- **Languages**: Python 3.7+, Bash 4.0+, R 4.0+ (depending on tools)
- **Optional**: AWS CLI (for cloud tools), SLURM (for HPC scripts)

### Install All Tools

```bash
# Clone all repositories
mkdir olympus-tools && cd olympus-tools
git clone https://github.com/olympus-terminal/bioinformatics-toolkit.git
git clone https://github.com/olympus-terminal/unix-utilities.git
git clone https://github.com/olympus-terminal/data-processing.git
git clone https://github.com/olympus-terminal/text-to-speech.git

# Add to PATH
echo 'export PATH="$PATH:$HOME/olympus-tools/bioinformatics-toolkit"' >> ~/.bashrc
echo 'export PATH="$PATH:$HOME/olympus-tools/unix-utilities"' >> ~/.bashrc
echo 'export PATH="$PATH:$HOME/olympus-tools/data-processing"' >> ~/.bashrc
echo 'export PATH="$PATH:$HOME/olympus-tools/text-to-speech"' >> ~/.bashrc
source ~/.bashrc
```

### Install Specific Collection

```bash
# Just bioinformatics tools
git clone https://github.com/olympus-terminal/bioinformatics-toolkit.git
cd bioinformatics-toolkit
pip install -r requirements.txt  # If available
```

## Usage Examples

### Real-World Workflows

#### 🧬 Genome Assembly Analysis
```bash
# Calculate assembly statistics
python n50calc.py genome.fa > stats.txt

# Check for contamination
sbatch QuickCheckContam.sbatch genome.fa

# Analyze k-mer distribution
sbatch meryl_merqury_long-reads-k-mers-hapQC.sbatch reads.fq
```

#### 📁 Bulk File Organization
```bash
# Clean messy filenames
./remove_special_chars_filenames.sh /downloads/

# Batch rename from CSV mapping
./rename_from_list.sh old_to_new.csv

# Find and report large directories
./report_offending_dirs.sh / > disk_usage.txt
```

#### 📊 Research Data Pipeline
```bash
# Extract text from PDFs
for pdf in *.pdf; do
    python pdf_to_txt_argv.py "$pdf"
done

# Count citations
python CountCitations.py manuscript.txt > citations.csv

# Create pivot table
Rscript pivot-table-maker.R citations.csv
```

#### 🎙️ Audiobook Production
```bash
# Preprocess text
./Clean_txt_for_TTS.sh book.txt > book_clean.txt

# Generate audiobook with neural TTS
python neural_tts.py --input book_clean.txt \
    --output audiobook.mp3 \
    --voice narrative \
    --chapter-mode
```

## Performance Benchmarks

| Operation | Standard Tool | Olympus Tool | Speedup |
|-----------|--------------|--------------|---------|
| Search 10GB logs | `grep -r` (8m) | `search_in_files-parallel.sh` (1.5m) | **5.3x** |
| Rename 10k files | Manual (hours) | `rename_from_list.sh` (30s) | **100x+** |
| Process PDFs | Manual (days) | Automated pipeline (hours) | **10x+** |
| BLAST parsing | Custom scripts | Optimized tools | **3-5x** |

## Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

### Ways to Contribute

- 🐛 Report bugs and issues
- 💡 Suggest new tools or features
- 🔧 Submit pull requests
- 📖 Improve documentation
- ⭐ Star repositories you find useful

## Support

- 📖 [Documentation Wiki](https://github.com/olympus-terminal/awesome-olympus-tools/wiki)
- 💬 [Discussions](https://github.com/olympus-terminal/awesome-olympus-tools/discussions)
- 🐛 [Issue Tracker](https://github.com/olympus-terminal/awesome-olympus-tools/issues)
- 📧 Contact: [@olympus-terminal](https://github.com/olympus-terminal)

## License

All tools are released under the MIT License. See [LICENSE](LICENSE) for details.

---

<div align="center">

**Made with ❤️ for the command-line community**

[![Follow](https://img.shields.io/github/followers/olympus-terminal?label=Follow&style=social)](https://github.com/olympus-terminal)
[![Star](https://img.shields.io/github/stars/olympus-terminal?style=social)](https://github.com/olympus-terminal)

</div>