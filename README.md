package com.klef.fsad.exam;

import jakarta.persistence.*;
import java.util.Date;

@Entity
@Table(name="invoice")
public class Invoice
{
    @Id
    @GeneratedValue(strategy=GenerationType.IDENTITY)
    private int id;

    private String name;
    private String status;
    private Date date;

    public Invoice() {}

    public Invoice(String name,String status,Date date)
    {
        this.name=name;
        this.status=status;
        this.date=date;
    }

    public int getId() { return id; }
    public String getName() { return name; }
    public String getStatus() { return status; }
    public Date getDate() { return date; }

    public void setName(String name){ this.name=name; }
    public void setStatus(String status){ this.status=status; }
    public void setDate(Date date){ this.date=date; }
}# fsad-in-sem-lab-exam
