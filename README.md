# fisher
A convinient tool for item extracting with different format such as table, fasta, fastq

# fisher

Description:  
        The design philosophy of brentcaodeng fisher.pl is of great importance in our daily work.  
        Say thanks to my best enlightened tutor and friend brentcaodeng.  
        I reimplemented this script based on my own logic.  
                                                                      --By CongfanBu  
                                                                      2019-10-30  
                                                                      qwerpoiupk@126.com  

                                                                      
Version:  
        1.3, In table mode, the fc and bc can be format customized  

        
Usage:  
  % fishInWinter.pl [options] <bait_file> <fish_file>  
    --bformat  <str>    set bait file format, fasta|table|fq  
    --fformat  <str>    set fish file format, fasta|table|gff|fq|gff3|gtf|vcf  
    --bcolumn  <num>    set bait file column, default=1, or it can be 1:3-4 customized  
    --fcolumn  <num>    set fish file column, default=1, or it can be 1:3-4 customized  
    --except   <boo>    get things not in the bait file  
    --maxcount <int>    stop after NUM matches  
    --split    <str>    separator when fisher, [table]or [space], default=table  
    --test     <boo>    output bc and fc contant to test  
    --nongreed <boo>    only print minimum number of coincident line, which very adapt that query is uniq in subject  
    --version  <boo>    print version and change log  
    --note     <boo>    also print #  


                        
Notes:  
        Due to time constraints, --nonpreed and --maxcount are currently only implemented in Fasta and Table (version 1.2)  
        Use the Nongreed parameter with caution unless you are sure of the exact number in the pool  
        The --maxcount and --nongreed may be used together to maximize fishing speed  
        The except parameter does not support nongreed matching
