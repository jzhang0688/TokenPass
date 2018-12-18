package com.company;

public class TokenRunner {

    public static void main(String[] args) {
	   TokenPass testGame = new TokenPass(10);
	   int [] testBoard = testGame.getBoard();
	   System.out.println("Constructed a testBoard: ");
	   for (int i = 0; i < testBoard.length; i++) {
           System.out.println(testBoard[i] + "");
       }
       System.out.println();
	   testGame.distributeCurrentPlayerTokens();
	   System.out.println("After distributing tokens from player " + testGame.getCurrentPlayer() + ": ");
	   for(int i = 0; i < testBoard.length; i++)
       {
           System.out.print(testBoard[i] + "");
       }
    }
}


package com.company;

public class TokenPass {
    private int PlayerCount;
    public TokenPass(int PlayerCount)
    {
        this.PlayerCount = PlayerCount;
    }
}


