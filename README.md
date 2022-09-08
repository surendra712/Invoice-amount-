class Invoice
{
  private String part_number;
  private String part_description;
  private int quality;
  private double price_item;
  private double total=0;
  Invoice ()
  {
    String part_number=" ";
    String part_description=" ";
    int quantity=0;
    double price_item=0.0;
  }
  public String getPart_number()
  { 
    return part_number;
  }
  public void setPart_number(String part_number)
  {
    this.part_number=part_number;
  } 
  public String getPart_description()
  {
    return part_description;
  }
  public void setPart_description(String part_description)
  {
    this.part_description=part_description;
  }
  public int getQuantity()
  {
    return quantity;
  }
  public void set Quantity (int quantity)
  {
    if (quantity<0)
    { 
      quantity=0;
    }
    else 
      this.quantity=quantity;
  }
  public double getPrice_item()
  {
    return price_item;
  }
  public void set price_item(double price_item)
  {
    if(price_item<0)
    {
      price_item=0.0;
    }
    else 
      this.price_item=price_item();
  }
  double getInvoiceAmount()
  {
    total price();
    return total;
  }
  void totalprice()
  {
    total=total+getQuantity ()*getPrice_item();
   }
}
class Program1
{
  public static void main(String arts[])
  {
    Scanner sc=new Scanner (System.in);
    Invoice in=new Invoice ();
    System.out.print("Enter part number:");
    in.setPart_number(sc.nexline());
    System.out.print("Enter no.of items purchased:");
    in.setQuality(sc.nextInt());
    System.out.print("Enter price per item :");
    in.setPrice_item(sc.nextDouble());
    System.out.print("Item details\n");
    System.out.print("Part number:"+in.getPart_number);
    System.out.print("Part description:"+in.getPart_description);
    System.out.print("\nTotal Billing Amount:"+in.getInvoiceAmount());
   }
 }



      
      
