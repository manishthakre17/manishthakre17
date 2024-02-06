public class FileRead {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
    try {
      File myObj = new File("C:\\Users\\sterl\\OneDrive\\Desktop\\new1.txt");
      Scanner myReader = new Scanner(myObj);
      while (myReader.hasNextLine()) {
        String data = myReader.nextLine();
        data=data.replace("\t", " ");
        System.out.println(data);
      }
      myReader.close();
    } catch (FileNotFoundException e) {
      System.out.println("An error occurred.");
      e.printStackTrace();
    }
  }
}

how can I improve this code
