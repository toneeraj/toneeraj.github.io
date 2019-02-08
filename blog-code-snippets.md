##Spring Batch

###custom process
```java

public class BirthdayFilterProcessor implements ItemProcessor<Customer, Customer> {
    @Override
    public Customer process(final Customer item) throws Exception {
        if (new GregorianCalendar().get(Calendar.MONTH) == item.getBirthday().get(Calendar.MONTH)) {
            log.info("Customer {} matched the birthday filter", item);
            return item;
        }
        return null;
    }

```
