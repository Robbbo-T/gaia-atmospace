# GAIA-QAO - The Unified Aerospace Vanguard Nexus

*Orchestrating identity, ethics, and operational intelligence across **Air ✈️ · Space 🛰️ · Greentech 🌱.***

---

### GAIA Platforms - Model Freezing Contexts (MFC) Controlled Vocabulary

*GenAI Proposal Status: This document was generated using AI assistance and represents a proposed controlled vocabulary for the MFC segment of the GAIA Platforms filename convention. It requires review and approval by the GP-FD team before implementation.*

## 1. Introduction

This document defines the official controlled vocabulary for the Model Freezing Context (MFC) segment of the GAIA Platforms filename convention. The MFC represents a specific, defined state or context within a lifecycle or design model at which the information contained in the document was "frozen" or established.

## 2. MFC Code Structure

Each MFC code follows this structure:

- Uppercase letters and underscores only
- Prefix indicates lifecycle phase
- Suffix indicates specific milestone or baseline
- Format: `PHASE_MILESTONE`


## 3. Controlled Vocabulary by Lifecycle Phase

### 3.1 Conceptual & Design Phase (CON_)

| MFC Code | Description | Typical Usage
|-----|-----|-----
| `CON_REQT` | Requirements Baseline | Initial requirements documentation
| `CON_ARCH` | Architecture Baseline | System architecture definition
| `CON_PDR` | Preliminary Design Review | Documentation approved at PDR
| `CON_CDR` | Critical Design Review | Documentation approved at CDR
| `CON_FREEZE_A` | Design Freeze Alpha | First formal design baseline
| `CON_FREEZE_B` | Design Freeze Beta | Second formal design baseline
| `CON_FREEZE_F` | Design Freeze Final | Final design baseline before implementation


### 3.2 Development Phase (DEV_)

| MFC Code | Description | Typical Usage
|-----|-----|-----
| `DEV_PROTO_A` | Prototype Alpha | First prototype documentation
| `DEV_PROTO_B` | Prototype Beta | Refined prototype documentation
| `DEV_IMPL_A` | Implementation Alpha | Initial implementation documentation
| `DEV_IMPL_B` | Implementation Beta | Refined implementation documentation
| `DEV_IMPL_F` | Implementation Final | Final implementation documentation
| `DEV_INT_A` | Integration Alpha | Initial integration documentation
| `DEV_INT_F` | Integration Final | Final integration documentation
| `DEV_TRR` | Test Readiness Review | Documentation approved at TRR


### 3.3 Testing Phase (TEST_)

| MFC Code | Description | Typical Usage
|-----|-----|-----
| `TEST_UNIT` | Unit Testing | Unit test documentation
| `TEST_INT` | Integration Testing | Integration test documentation
| `TEST_SYS` | System Testing | System test documentation
| `TEST_ENV` | Environmental Testing | Environmental test documentation
| `TEST_PERF` | Performance Testing | Performance test documentation
| `TEST_SAFE` | Safety Testing | Safety test documentation
| `TEST_QUAL` | Qualification Testing | Qualification test documentation
| `TEST_ACCEPT` | Acceptance Testing | Acceptance test documentation


### 3.4 Certification Phase (CERT_)

| MFC Code | Description | Typical Usage
|-----|-----|-----
| `CERT_PLAN` | Certification Planning | Certification planning documentation
| `CERT_SUBMIT` | Certification Submittal | Documentation submitted for certification
| `CERT_REVIEW` | Certification Review | Documentation under certification review
| `CERT_COMPLY` | Certification Compliance | Documentation demonstrating compliance
| `CERT_FINAL` | Certification Final | Final certified documentation
| `CERT_TYPE` | Type Certification | Type certification documentation
| `CERT_PROD` | Production Certification | Production certification documentation
| `CERT_AIRW` | Airworthiness Certification | Airworthiness certification documentation


### 3.5 Production Phase (PROD_)

| MFC Code | Description | Typical Usage
|-----|-----|-----
| `PROD_TOOL` | Production Tooling | Tooling documentation
| `PROD_PROC` | Production Processes | Manufacturing process documentation
| `PROD_QA` | Quality Assurance | QA documentation
| `PROD_FIRST` | First Article | First article inspection documentation
| `PROD_BATCH` | Batch Production | Batch production documentation
| `PROD_MOD_A` | Production Modification Alpha | Initial production modification
| `PROD_MOD_B` | Production Modification Beta | Secondary production modification
| `PROD_MOD_F` | Production Modification Final | Final production modification


### 3.6 Operational Phase (OPS_)

| MFC Code | Description | Typical Usage
|-----|-----|-----
| `OPS_DEPLOY` | Initial Deployment | Initial deployment documentation
| `OPS_BASE_A` | Operational Baseline Alpha | First operational baseline
| `OPS_BASE_B` | Operational Baseline Beta | Second operational baseline
| `OPS_BASE_F` | Operational Baseline Final | Final operational baseline
| `OPS_CONFIG_A` | Configuration Alpha | First operational configuration
| `OPS_CONFIG_B` | Configuration Beta | Second operational configuration
| `OPS_CONFIG_F` | Configuration Final | Final operational configuration
| `OPS_UPDATE` | Operational Update | Operational update documentation


### 3.7 Maintenance Phase (MAINT_)

| MFC Code | Description | Typical Usage
|-----|-----|-----
| `MAINT_PLAN` | Maintenance Planning | Maintenance planning documentation
| `MAINT_SCHED` | Scheduled Maintenance | Scheduled maintenance documentation
| `MAINT_UNSCHED` | Unscheduled Maintenance | Unscheduled maintenance documentation
| `MAINT_PROC_A` | Maintenance Procedure Alpha | Initial maintenance procedure
| `MAINT_PROC_V` | Maintenance Procedure Validated | Validated maintenance procedure
| `MAINT_PROC_F` | Maintenance Procedure Final | Final maintenance procedure
| `MAINT_SB` | Service Bulletin | Service bulletin documentation
| `MAINT_MOD` | Modification | Modification documentation


### 3.8 Retirement & Disposal Phase (EOL_)

| MFC Code | Description | Typical Usage
|-----|-----|-----
| `EOL_PLAN` | End-of-Life Planning | EOL planning documentation
| `EOL_DECOM` | Decommissioning | Decommissioning documentation
| `EOL_DISASM` | Disassembly | Disassembly documentation
| `EOL_RECYCLE` | Recycling | Recycling documentation
| `EOL_DISPOSE` | Disposal | Disposal documentation
| `EOL_ARCHIVE` | Archiving | Archiving documentation
| `EOL_LEGACY` | Legacy Support | Legacy support documentation
| `EOL_HIST` | Historical Record | Historical record documentation


## 4. Domain-Specific MFC Codes

### 4.1 AIR Domain Specific

| MFC Code | Description | Typical Usage
|-----|-----|-----
| `AIR_FLIGHT_TEST` | Flight Testing | Flight test documentation
| `AIR_ETOPS` | ETOPS Certification | ETOPS certification documentation
| `AIR_RVSM` | RVSM Certification | RVSM certification documentation
| `AIR_MEL` | Minimum Equipment List | MEL documentation
| `AIR_AD` | Airworthiness Directive | AD documentation


### 4.2 SPACE Domain Specific

| MFC Code | Description | Typical Usage
|-----|-----|-----
| `SPACE_LAUNCH_QUAL` | Launch Qualification | Launch qualification documentation
| `SPACE_FRR` | Flight Readiness Review | FRR documentation
| `SPACE_MISSION_A` | Mission Phase Alpha | Initial mission phase documentation
| `SPACE_MISSION_B` | Mission Phase Beta | Secondary mission phase documentation
| `SPACE_EOL` | End-of-Life Operations | Space system EOL documentation


### 4.3 GREENTECH Domain Specific

| MFC Code | Description | Typical Usage
|-----|-----|-----
| `GREEN_IMPACT` | Environmental Impact | Environmental impact documentation
| `GREEN_CARBON` | Carbon Assessment | Carbon assessment documentation
| `GREEN_LIFECYCLE` | Lifecycle Assessment | Lifecycle assessment documentation
| `GREEN_SUSTAIN` | Sustainability Review | Sustainability review documentation
| `GREEN_CIRCULAR` | Circular Economy | Circular economy documentation


## 5. Cross-Domain MFC Codes

| MFC Code | Description | Typical Usage
|-----|-----|-----
| `X_BASELINE` | Cross-Domain Baseline | Baseline applicable across domains
| `X_STANDARD` | Standardization | Documentation of standardized components
| `X_INTERFACE` | Interface Control | Interface control documentation
| `X_SAFETY` | Safety Critical | Safety critical documentation
| `X_SECURITY` | Security Critical | Security critical documentation


## 6. Implementation Guidelines

### 6.1 MFC Selection Rules

1. Select the most specific applicable MFC code
2. Use phase-specific codes when the document relates to a specific lifecycle phase
3. Use domain-specific codes when the document is unique to a domain
4. Use cross-domain codes when the document applies across domains
5. When multiple codes could apply, select the one representing the primary purpose


### 6.2 Examples

| Filename | Description
|-----|-----|-----
| `CON_FREEZE_B_AMPEL_27-20-15_RUDDER_ACTUATOR_SPEC_A.md` | Rudder actuator specification at Design Freeze Beta
| `MAINT_PROC_V_AMPEL_24-60-10_PMSC_REMOVAL_PROC_C.xml` | Validated maintenance procedure for PMSC removal
| `CERT_AIRW_FW-CT-LCA_53-10-00_NOSE_RADOME_CERT_B.pdf` | Airworthiness certification for commercial transport aircraft nose radome
| `TEST_ENV_GP-SS_05-10-20_SOLAR_ARRAY_TST_001.yaml` | Environmental test documentation for space system solar array
| `GREEN_LIFECYCLE_RE-WE_01-20-30_TURBINE_BLADE_LCA_A.xml` | Lifecycle assessment for wind turbine blade


### 6.3 Validation Rules

1. MFC code must be from the controlled vocabulary
2. MFC code must be appropriate for the document type
3. MFC code must be appropriate for the platform class
4. MFC code must be appropriate for the lifecycle phase


## 7. Governance and Maintenance

1. This controlled vocabulary is maintained by the GP-FD Documentation Standards Committee
2. New MFC codes must be proposed and approved through the standard change process
3. MFC codes may be deprecated but should never be removed
4. Annual review of the MFC controlled vocabulary will be conducted

#!/usr/bin/env python3
"""
GAIA Platforms Filename Validator (Enhanced)

This script validates filenames against the GAIA Platforms filename convention:
[MFC]_[PlatformClass]_[SNS_Code]_[Descriptor]_[InfoCode]_[Revision].[Ext]

Usage:
    python validate_filenames.py [directory]
    python validate_filenames.py [file1] [file2] ...
    python validate_filenames.py --check-metadata [directory]
"""

import os
import re
import sys
import argparse
import yaml
from pathlib import Path
from typing import Dict, List, Set, Tuple, Optional, Union

# Define the controlled vocabulary for MFC codes
MFC_CODES = {
    # Conceptual & Design Phase
    "CON_REQT", "CON_ARCH", "CON_PDR", "CON_CDR", 
    "CON_FREEZE_A", "CON_FREEZE_B", "CON_FREEZE_F",
    
    # Development Phase
    "DEV_PROTO_A", "DEV_PROTO_B", "DEV_IMPL_A", "DEV_IMPL_B", 
    "DEV_IMPL_F", "DEV_INT_A", "DEV_INT_F", "DEV_TRR",
    
    # Testing Phase
    "TEST_UNIT", "TEST_INT", "TEST_SYS", "TEST_ENV", 
    "TEST_PERF", "TEST_SAFE", "TEST_QUAL", "TEST_ACCEPT",
    
    # Certification Phase
    "CERT_PLAN", "CERT_SUBMIT", "CERT_REVIEW", "CERT_COMPLY", 
    "CERT_FINAL", "CERT_TYPE", "CERT_PROD", "CERT_AIRW",
    
    # Production Phase
    "PROD_TOOL", "PROD_PROC", "PROD_QA", "PROD_FIRST", 
    "PROD_BATCH", "PROD_MOD_A", "PROD_MOD_B", "PROD_MOD_F",
    
    # Operational Phase
    "OPS_DEPLOY", "OPS_BASE_A", "OPS_BASE_B", "OPS_BASE_F", 
    "OPS_CONFIG_A", "OPS_CONFIG_B", "OPS_CONFIG_F", "OPS_UPDATE",
    
    # Maintenance Phase
    "MAINT_PLAN", "MAINT_SCHED", "MAINT_UNSCHED", "MAINT_PROC_A", 
    "MAINT_PROC_V", "MAINT_PROC_F", "MAINT_SB", "MAINT_MOD",
    
    # Retirement & Disposal Phase
    "EOL_PLAN", "EOL_DECOM", "EOL_DISASM", "EOL_RECYCLE", 
    "EOL_DISPOSE", "EOL_ARCHIVE", "EOL_LEGACY", "EOL_HIST",
    
    # AIR Domain Specific
    "AIR_FLIGHT_TEST", "AIR_ETOPS", "AIR_RVSM", "AIR_MEL", "AIR_AD",
    
    # SPACE Domain Specific
    "SPACE_LAUNCH_QUAL", "SPACE_FRR", "SPACE_MISSION_A", 
    "SPACE_MISSION_B", "SPACE_EOL",
    
    # GREENTECH Domain Specific
    "GREEN_IMPACT", "GREEN_CARBON", "GREEN_LIFECYCLE", 
    "GREEN_SUSTAIN", "GREEN_CIRCULAR",
    
    # Cross-Domain
    "X_BASELINE", "X_STANDARD", "X_INTERFACE", "X_SAFETY", "X_SECURITY"
}

# Define the controlled vocabulary for InfoCodes
INFO_CODES = {
    "SPEC", "PROC", "IPD", "CAD", "DWG", "BOM", "TST", "MAINT", 
    "SIM", "CERT", "RISK", "LCA", "SUST", "AIRW", "FT", "RAD", 
    "ODEB", "SCHEMA"
}

# Define the controlled vocabulary for Platform Classes
VALID_PLATFORM_CLASSES = {
    # AIR Domain
    ## AMPEL Family
    "AMPEL", "AMPELPLUS", "AMPEL-CARGO", "AMPEL-PAX",
    
    ## Fixed Wing Aircraft
    "FW-CT-LCA", "FW-CT-MCA", "FW-CT-RCA",  # Commercial Transport (Large/Medium/Regional)
    "FW-GA-LA", "FW-GA-MA", "FW-GA-SA",     # General Aviation (Large/Medium/Small)
    "FW-ML-FTR", "FW-ML-ATK", "FW-ML-TRN",  # Military (Fighter/Attack/Trainer)
    
    ## Rotary Wing Aircraft
    "RW-HC-LH", "RW-HC-MH", "RW-HC-LH",     # Helicopter (Light/Medium/Heavy)
    "RW-ML-ATK", "RW-ML-UTL", "RW-ML-TRN",  # Military Rotorcraft
    
    ## Advanced Mobility
    "AM-EV-AT", "AM-EV-MT", "AM-EV-LT",     # eVTOL (Air Taxi/Metro/Logistics)
    "AM-UA-SM", "AM-UA-MD", "AM-UA-LG",     # UAV/UAS (Small/Medium/Large)
    
    # SPACE Domain
    ## Launch Vehicles
    "LV-RL-FR", "LV-RL-HR", "LV-RL-SR",     # Rocket Launch (Full/Heavy/Small)
    "LV-AL-SS", "LV-AL-OS",                 # Air Launch (Suborbital/Orbital)
    
    ## Spacecraft
    "SC-SA-COMM", "SC-SA-EO", "SC-SA-NAV",  # Satellite (Communications/Earth Observation/Navigation)
    "SC-HS-CC", "SC-HS-SM", "SC-HS-HM",     # Human Spaceflight (Crew Capsule/Station Module/Habitat Module)
    "SC-RP-OM", "SC-RP-PM", "SC-RP-LM",     # Robotic Probe (Orbital/Planetary/Lunar)
    
    ## Orbital Infrastructure
    "OI-SS-PM", "OI-SS-HM", "OI-SS-SM",     # Space Station (Power Module/Habitat Module/Service Module)
    "OI-SV-RM", "OI-SV-FM",                 # Servicing Vehicle (Refueling Module/Repair Module)
    
    # GREENTECH Domain
    ## Renewable Energy
    "RE-WE-HAWT", "RE-WE-VAWT", "RE-WE-OFF", # Wind Energy (Horizontal Axis/Vertical Axis/Offshore)
    "RE-SE-PV", "RE-SE-CSP", "RE-SE-CPV",   # Solar Energy (Photovoltaic/Concentrated Solar Power/Concentrated PV)
    "RE-HE-ROR", "RE-HE-DAM", "RE-HE-TID",  # Hydro Energy (Run-of-River/Dam/Tidal)
    
    ## Energy Storage
    "ES-BS-LI", "ES-BS-SS", "ES-BS-FL",     # Battery Storage (Lithium/Solid State/Flow)
    "ES-HS-PH", "ES-HS-CA", "ES-HS-TH",     # Hydrogen Storage (Pressure/Cryogenic/Metal Hydride)
    "ES-TS-PCM", "ES-TS-TES", "ES-TS-CAES", # Thermal Storage (Phase Change/Thermal/Compressed Air)
    
    ## Sustainable Materials
    "SM-BM-BP", "SM-BM-BC", "SM-BM-BF",     # Biomaterials (Bioplastics/Biocomposites/Biofibers)
    "SM-RM-RP", "SM-RM-RM", "SM-RM-RE",     # Recycled Materials (Plastics/Metals/Electronics)
    "SM-AM-LW", "SM-AM-HS", "SM-AM-SF",     # Advanced Materials (Lightweight/High Strength/Self-healing)
    
    # Infrastructure & Systems
    "DOCSYS-DB", "DOCSYS-API", "DOCSYS-UI", # Documentation System
    "DEVSYS-CI", "DEVSYS-VCS", "DEVSYS-PM", # Development Systems
    "SIMSYS-DT", "SIMSYS-VR", "SIMSYS-CFD", # Simulation Systems
    
    # Cross-Domain & Foundation
    "GP-FD", "GP-SS", "GP-AIR", "GP-GREEN", # GAIA Platforms Foundation/Shared Services
    "X-STANDARD", "X-INTERFACE", "X-SAFETY" # Cross-domain standards
}

# Define the pattern for SNS codes
SNS_CODE_PATTERN = r'\d{2}-\d{2}-\d{2}(-\d{3})?'

# Define the pattern for the entire filename
FILENAME_PATTERN = (
    r'^([A-Z][A-Z0-9_]+)_'           # MFC
    r'([A-Z][A-Z0-9_-]+)_'           # PlatformClass
    r'(\d{2}-\d{2}-\d{2}(?:-\d{3})?)_' # SNS_Code
    r'([A-Z][A-Z0-9_]+)_'            # Descriptor
    r'([A-Z][A-Z0-9_]+)_'            # InfoCode
    r'([A-Z0-9]+)'                   # Revision
    r'\.([a-z0-9]+)$'                # Extension
)

def validate_filename(filename: str) -> Tuple[bool, List[str]]:
    """
    Validate a filename against the GAIA Platforms filename convention.
    
    Args:
        filename: The filename to validate
        
    Returns:
        Tuple of (is_valid, list_of_errors)
    """
    errors = []
    
    # Check if the filename matches the pattern
    match = re.match(FILENAME_PATTERN, filename)
    if not match:
        errors.append(f"Filename does not match the required pattern: {FILENAME_PATTERN}")
        return False, errors
    
    # Extract components
    mfc, platform_class, sns_code, descriptor, info_code, revision, extension = match.groups()
    
    # Validate MFC
    if mfc not in MFC_CODES:
        errors.append(f"Invalid MFC code: {mfc}. Must be one of the controlled vocabulary.")
    
    # Validate PlatformClass
    if platform_class not in VALID_PLATFORM_CLASSES:
        errors.append(f"Invalid PlatformClass code: '{platform_class}'. Must be one of the controlled vocabulary.")
    
    # Validate SNS code
    if not re.match(SNS_CODE_PATTERN, sns_code):
        errors.append(f"Invalid SNS code: {sns_code}. Must match pattern: {SNS_CODE_PATTERN}")
    
    # Validate InfoCode
    if info_code not in INFO_CODES:
        errors.append(f"Invalid InfoCode: {info_code}. Must be one of the controlled vocabulary.")
    
    # Validate Descriptor (just check it's not empty and is uppercase with underscores)
    if not descriptor or not re.match(r'^[A-Z][A-Z0-9_]+$', descriptor):
        errors.append(f"Invalid Descriptor: {descriptor}. Must be uppercase with underscores.")
    
    # Validate Revision (just check it's not empty)
    if not revision:
        errors.append("Revision cannot be empty.")
    
    # Validate Extension (just check it's not empty)
    if not extension:
        errors.append("Extension cannot be empty.")
    
    return len(errors) == 0, errors

def check_metadata_file(filename: str) -> Tuple[bool, List[str]]:
    """
    Check if a metadata file exists for the given filename and validate its content.
    
    Args:
        filename: The filename to check for metadata
        
    Returns:
        Tuple of (has_valid_metadata, list_of_errors)
    """
    errors = []
    
    # Determine the metadata filename (same name but with .yaml extension)
    base_name = os.path.splitext(filename)[0]
    metadata_filename = f"{base_name}.yaml"
    
    # Check if the metadata file exists
    if not os.path.exists(metadata_filename):
        errors.append(f"Metadata file not found: {metadata_filename}")
        return False, errors
    
    # Load and validate the metadata
    try:
        with open(metadata_filename, 'r') as f:
            metadata = yaml.safe_load(f)
        
        # Check required fields
        required_fields = [
            "document_id", "title", "description", "classification", 
            "trl", "status", "revision_history"
        ]
        
        for field in required_fields:
            if field not in metadata:
                errors.append(f"Missing required metadata field: {field}")
        
        # Check that document_id matches the filename
        if "document_id" in metadata and metadata["document_id"] != os.path.basename(filename):
            errors.append(f"Metadata document_id ({metadata['document_id']}) does not match filename ({os.path.basename(filename)})")
        
    except Exception as e:
        errors.append(f"Error reading metadata file: {str(e)}")
        return False, errors
    
    return len(errors) == 0, errors

def process_file(filepath: str, check_metadata: bool = False) -> Tuple[bool, List[str]]:
    """
    Process a single file, validating its filename and optionally its metadata.
    
    Args:
        filepath: Path to the file to process
        check_metadata: Whether to also check for a valid metadata file
        
    Returns:
        Tuple of (is_valid, list_of_errors)
    """
    filename = os.path.basename(filepath)
    is_valid, errors = validate_filename(filename)
    
    if check_metadata and is_valid:
        metadata_valid, metadata_errors = check_metadata_file(filepath)
        is_valid = is_valid and metadata_valid
        errors.extend(metadata_errors)
    
    return is_valid, errors

def process_directory(directory: str, check_metadata: bool = False) -> Dict[str, List[str]]:
    """
    Process all files in a directory, validating filenames and optionally metadata.
    
    Args:
        directory: Directory to process
        check_metadata: Whether to also check for valid metadata files
        
    Returns:
        Dictionary mapping filenames to lists of errors
    """
    results = {}
    
    for root, _, files in os.walk(directory):
        for filename in files:
            # Skip metadata files and hidden files
            if filename.endswith('.yaml') or filename.startswith('.'):
                continue
                
            filepath = os.path.join(root, filename)
            is_valid, errors = process_file(filepath, check_metadata)
            
            if not is_valid:
                results[filepath] = errors
    
    return results

def main():
    parser = argparse.ArgumentParser(description='Validate filenames against GAIA Platforms convention')
    parser.add_argument('paths', nargs='+', help='Files or directories to validate')
    parser.add_argument('--check-metadata', action='store_true', help='Also check for valid metadata files')
    parser.add_argument('--list-platform-classes', action='store_true', help='List all valid platform classes')
    parser.add_argument('--list-mfc-codes', action='store_true', help='List all valid MFC codes')
    parser.add_argument('--list-info-codes', action='store_true', help='List all valid InfoCodes')
    
    args = parser.parse_args()
    
    # Handle listing of controlled vocabularies
    if args.list_platform_classes:
        print("\nValid Platform Classes:")
        for platform_class in sorted(VALID_PLATFORM_CLASSES):
            print(f"  {platform_class}")
        return
    
    if args.list_mfc_codes:
        print("\nValid MFC Codes:")
        for mfc_code in sorted(MFC_CODES):
            print(f"  {mfc_code}")
        return
    
    if args.list_info_codes:
        print("\nValid InfoCodes:")
        for info_code in sorted(INFO_CODES):
            print(f"  {info_code}")
        return
    
    all_results = {}
    
    for path in args.paths:
        if os.path.isdir(path):
            results = process_directory(path, args.check_metadata)
            all_results.update(results)
        elif os.path.isfile(path):
            is_valid, errors = process_file(path, args.check_metadata)
            if not is_valid:
                all_results[path] = errors
        else:
            print(f"Error: Path not found: {path}")
    
    # Print results
    if all_results:
        print(f"\n{len(all_results)} files with errors found:")
        for filepath, errors in all_results.items():
            print(f"\n{filepath}:")
            for error in errors:
                print(f"  - {error}")
        sys.exit(1)
    else:
        print("All filenames are valid!")
        sys.exit(0)

if __name__ == "__main__":
    main()
---

*Document ID: X_STANDARD_GP-DOC_00-00-00_MFC_VOCABULARY_A.md**Last Updated: 2025-05-01*

