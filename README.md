# Test_FileBitwisePartition
Initial file bitwise partition project


This is an initial trial of FileBitwisePartition project.

The idea is partitioning data of file at the byte level, so that each partition
of a file only hold partial data which cannot be review or decoded by others to 
retrieve the original information content stored in the file.

The way of partitioning a file at the byte level, divides all bytes into bits,
that information represented in bytes, cannot be decoded.  For an example, if 
a file, consisting only one byte, is partitioned into two parts, one is the
higher 4 bits, the other is lower 4 bits.  Thus, revealing only one part of
of the byte would not be able lead to full 8-bit information. Only when
the two parts are reassembled into a 8-bit byte, content can be revealed.

There are different methods under consideration how bytes can be partitioned.
In different words, we reshaffle the data based on bits address into different
segements.  