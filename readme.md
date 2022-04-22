# HW 10
## Violet Smith
### April 19th, 2020

#### 1. Is it fundamentally necessary to store on disk the information about the unallocated disk sectors? Explain why.

<p> It is not fundamentally necessary to store on disk the information about the unallocated disk. Storing this information is good practice though. It makes the job of utilities easier and the system is more secure. </p>

#### 2. In some early release of an operating system, when a file was deleted, its sectors reverted to the free list but they were not erased. What problems do you think may result from this? Why do you think the blocks were not erased?

<p> This would cause a securiy problem because users and attackers would be able to access deleted data in the free list if they could figure out how to access it. It could also retain user data and belong to the wrong person when over righting the file. The blocks were probably not erased due to them thinking it was a waste of time.  </p>

#### 3. You are designing a file system from scratch. The disk driver allows you complete control over the placement of data on the disk. Assuming that you have settled for a File Allocation Table (FAT) architecture, where would be the best place to store the table on disk?

<p> I would place the data that I am putting on the disk in the middle of the track in the disk. This is because under the scheduler policy that the FAT architecture uses the middle of the track would be the most efficient place to hold the data as it is visited twice by the disk head in one trip. It is also the fastest to reach compared to other places on the disk. </p>

#### 4. Contiguous allocation of files leads to disk fragmentation. Explain why?

<p> In the scope of contiguous allocation each process or file is contained in a single section of the disk memory. This means that all of the spaces allocated are the perfect size for the file they hold. When a file is then deleted the section on the disk where the file was held is now an empty chunck that can only be filled by a file of the same size or less. This leads to fragmentation because no one holds files that are all the exact same size. </p>

#### 5. Can we implement symbolic links in DOS (FAT file system)? If so, show how, and if not, explain why.

<p> We could inplement symbolic links in DOS by  </p> 
