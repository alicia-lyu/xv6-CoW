READ ME

* name: Alicia Lyu, Shuyao Li
* cs login: wenhui, ??
* wisc ID: wlyu27, ??
* email: wlyu27@wisc.edu, ??
* status of implementation: **fork test OK; all other tests passed except for #3.** (Legend: I think there is **a mistake in this test**. Briefly, I failed because the free pages of parent decreased by 1 after the child process is complete. However, I used gdb and found that only one kalloc is called during child process. I think *that page of the parent is allocated during fork() ( allocproc() involves kalloc() )*. My child proc didn't change free pages of the parent. I will write a piazza post tomorrow to address that detailedly.)