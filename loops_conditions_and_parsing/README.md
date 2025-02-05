# alu-shell

This repository contains a collection of Bash scripts for the ALU Shell project.

## Directory Structure

- **init_files_variables_and_expansions**: Contains scripts related to initialization, files, variables, and expansions.
- **loops_conditions_and_parsing**: Contains scripts demonstrating loops, conditional statements, parsing, and log processing.

## loops_conditions_and_parsing Scripts

- **1-for_best_school**: Displays "Best School" 10 times using a **for** loop.
- **2-while_best_school**: Displays "Best School" 10 times using a **while** loop.
- **3-until_best_school**: Displays "Best School" 10 times using an **until** loop.
- **4-if_9_say_hi**: Displays "Best School" 10 times using a **while** loop; on the 9th iteration, it also prints "Hi" on a new line.
- **5-4_bad_luck_8_is_your_chance**: Loops from 1 to 10 using a **while** loop with if/elif/else; displays "bad luck" for the 4th iteration, "good luck" for the 8th, and "Best School" for the others.
- **6-superstitious_numbers**: Displays numbers from 1 to 20 with special messages on the 4th, 9th, and 17th iterations using a **while** loop and a **case** statement.
- **7-clock**: Displays hours from 0 to 12 and, for each hour, minutes from 1 to 59 using nested **while** loops.
- **8-for_ls**: Displays the contents of the current directory (non-hidden) in a list format, showing only the part of the filename after the first dash.
- **9-to_file_or_not_to_file**: Checks for a file named "school" and reports whether it exists, if it's empty, and if it's a regular file.
- **10-fizzbuzz**: Displays numbers from 1 to 100 with FizzBuzz logic.
- **11-read_and_cut**: Displays selected fields (username, user id, home directory) from **/etc/passwd** using a **while** loop.
- **12-tell_the_story_of_passwd**: Tells a formatted story of each user in **/etc/passwd** using a **while** loop with IFS.
- **13-lets_parse_apache_logs**: Uses **awk** to extract the visitor IP and HTTP status code from the Apache log file.
- **14-dig_the-data**: Uses **awk** to group and sort Apache log entries by occurrence, displaying occurrence number, IP, and HTTP status code.

