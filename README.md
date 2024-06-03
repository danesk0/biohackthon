# Print ('More than cells') - Sequence Analysis Project

## Team Members
- Daniyar Yestay
- Temirlan Nurligenov
- Aidyn Tulepbergenov
- Ainur Aimurziyeva

## Task
The task is to perform sequence analysis by creating a program that identifies and modifies restriction sites within a DNA sequence without changing the amino acid sequence. This approach is similar to inducing silent mutations.

## Solution
We developed a Python program that:
1. Accepts a DNA sequence input from the user.
2. Identifies user-specified restriction sites within the sequence.
3. Alters one of the bases in the restriction site to hide it, ensuring the amino acid sequence remains unchanged.
4. Outputs the modified DNA sequence and its complementary strand.

## How the Code Works
1. **Input DNA Sequence:**
   - The program prompts the user to enter a DNA sequence. There are no restrictions on the type or length of the sequence.
   
2. **Specify Restriction Sites:**
   - The program asks the user how many types of restriction sites to find. The user enters an integer corresponding to the number of restriction sites.
   - The user then enters the base sequences of the required restriction sites sequentially.
   - Example: For EcoRI (GAATTC) and XbaI (TCTAGA), the user should enter 2 and then input the sequences GAATTC and TCTAGA respectively.
   
3. **Analyze and Modify Sequence:**
   - The program analyzes the DNA sequence to find all instances of the specified restriction sites.
   - It then modifies one base in each restriction site to hide it while ensuring the amino acid sequence remains unchanged.
   
4. **Output Results:**
   - The program outputs the modified DNA sequence and its complementary strand.

## Advantages
- **Precision in Mutation:** The program makes base changes that result in silent mutations, ensuring the amino acid sequence remains unchanged.
- **Flexibility:** Users can input any restriction site sequence, providing flexibility and avoiding limitations of standard choices.

## Future Improvements
- **Database for Restriction Sites:** Allow users to enter the name of a restriction site rather than its sequence by creating a comprehensive database of restriction sites, which can be updated with new information.
- **Detailed Analysis:** Provide exact positions and numbers of modified restriction sites to enhance the researcher's understanding of changes made.

## Usage for Researchers
- **Beyond Restriction Sites:** Since the program requires only sequence inputs, it can be used to induce silent mutations in any part of the DNA code, not just restriction sites.

## Code Description

### Input Data Validation
- Converts lowercase DNA sequences to uppercase.
- Ensures the input contains valid nucleobases only, prompting the user for a valid sequence if necessary.

### Restriction Site Validation
- Ensures restriction site sequences are at least 3 bases long and contain valid nucleobases, prompting for correct input if necessary.

### Silent Mutation Algorithm
- Identifies the restriction site in the DNA sequence.
- Changes a nucleobase in the restriction site to maintain the same amino acid sequence, effectively hiding the restriction site.

### Output Generation
- Outputs the modified DNA sequence.
- Generates and outputs the complementary strand for the final DNA sequence.
