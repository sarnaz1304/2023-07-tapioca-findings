It is irrelevant to have modifiers of no use in functions for instance as we can see in function repay inside SGLBorrow.sol, the function is meant to repay the borrowed amount so there is no point of checking whether he is allowed to borrow the particular amount in  allowedBorrow(from, part) modifier when he has got the amount already, this will save a lot of gas too.

https://github.com/Tapioca-DAO/tapioca-bar-audit/blob/2286f80f928f41c8bc189d0657d74ba83286c668/contracts/markets/singularity/SGLBorrow.sol#L50