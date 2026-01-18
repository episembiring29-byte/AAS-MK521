# AAS-MK521
AAS MK521
lot_processes = {
    'VF535361B06': 'Autovision',
    'VF534367B06': 'QC-GATE',
    'VF535361B05': 'Autovision',
    'VF534367B09': 'QC-GATE',
    'VF535317B14': 'Autovision'  # Corrected typo from 'Autovison'
}

def identify_process(lot_code):
    # First, check direct lookup
    if lot_code in lot_processes:
        return lot_processes[lot_code]
    # Fallback: Pattern-based (e.g., prefix matching)
    if lot_code.startswith('VF535'):
        return 'Autovision'
    elif lot_code.startswith('VF534'):
        return 'QC-GATE'
    else:
        return 'Unknown'
print("Lot Identification Results:")
print("-" * 40)
for lot in lots_to_check:
    process = identify_process(lot)
    print(f"Lot {lot}: Process {process}")
